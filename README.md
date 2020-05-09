# Usage
Clone the repository using 

```
git clone git@github.com:sarcaustech/vimeet-lets-go-docker-compose.git
```

and run the [git-clone.sh](/git-clone.sh) script to checkout Vimeet Server and Vimeet Let's Go plus copying the server's required .env file from template.

Start the setup with
```
docker-compose up
```
Depeding on you os setup, you might need to run this with higher privilidges.Vimeet will be available on port 8080.

To update Vimeet to the current master branches, run [update.sh](/update.sh).

To rebuild a specific service, run 
```
docker-compose build <SERVICE_NAME>
```

To complete rebuild Vimeet, run
```
docker-compose up --build
```

# Note
Make sure to have permissions to execute the scripts. If not, grant them, e.g. 
```
chmod u+x git-clone.sh
chmod u+x update.sh
```

# References
* [Vimeet Server](https://www.github.com/sarcaustech/vimeet-server)
* [Vimeet Let's Go](https://www.github.com/sarcaustech/vimeet-lets-go)
