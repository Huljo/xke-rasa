# Xebia Rasa NLU XKE

## Run
### To start Rasa NLU (Spacy) + Rasa UI run the following command :

```
docker-compose up
```

## Train

### Using Rasa ui
Got to http://localhost:5002/

### Using Rasa NLU http server ([https://nlu.rasa.com/http.html](https://nlu.rasa.com/http.html))
```
curl -XPOST -H "Content-Type: application/x-yml" localhost:5000/train?project=my_project \
    -d @config/config_train_server_md.yml
```

# Parse

```
 curl -XPOST localhost:5000/parse -d '{"q":"hello there"}'
```


---
## Rasa documentation : 
[https://nlu.rasa.com/](https://nlu.rasa.com/)
