# Project Title

**UPSCALEPICS API**


### Prerequisites

* A)Tensorflow >2.0
* B)Open CV
* C)Python3



### Installing

* Clone this repo or Download the zip file.
```
pip3 install -r requirements.txt
```
* Unzip ad run the script api.py
* It will start a local Flask Server

```
python3 api.py
```



## Running the tests

Then open another terminal and Call the api:

```
 curl -AT -F image=@image.png -F jpeg=True -F scale=2 -F user=spyne -F key=123  http://127.0.0.1:5000
```

It will give an output:

```
{"url": "url", "error": false}
```

### Break down into end to end tests

Input Parameters:
* **image**: The image file.
* **jpeg** : Weather jpeg removal is needed or not.
* **scale**: Scale of upscaling.
* **user** : The username of client.
* **key**  : The secret api Key.

Output :
**json**
keys:
* **url**: The url containiing processed images.
* **error**:Weather any error occured or not.



## Built With

* [Flask](http://www.dropwizard.io/1.0.2/docs/) - The web framework used
* [Tensorflow](https://maven.apache.org/) - AI Library
* [Open CV](https://rometools.github.io/rome/) - Used to generate RSS Feeds



## Authors

* **Debangshu Paul** - *Initial work* - [PurpleBooth](https://github.com/debangshu132)

See also the list of [contributors](https://github.com/your/project/contributors) who participated in this project.

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details

## Acknowledgments

* Anuj Agrawal
* Mukesh Babu
* Gyanendra Dubey

