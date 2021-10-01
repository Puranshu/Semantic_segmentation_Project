# Semantic segmentation

- This repository contain one [raw code file](https://github.com/Puranshu/Semantic_segmentation_Project/blob/main/Semantic%20Segmentation%20-%20Complete.ipynb) and [one errored file](https://github.com/Puranshu/Semantic_segmentation_Project/blob/main/Semantic%20Segmentation_Error.ipynb).

- Error occured while executing because : Service limit was reached for **trainingjob** instance, had = 0, required = 1.  

## Aim 
![Original](https://github.com/Puranshu/Semantic_segmentation_Project/blob/main/Original%20image.png) to ![Segmented](https://github.com/Puranshu/Semantic_segmentation_Project/blob/main/Segmented%20image.png)


## Roadmap

- First we create notebook instance on Amazon sagemaker and then we download and extract the data.

- The downloaded data can be found on jupyter notebook's directory.

- Then we vizualize the data to get a picture of our task.

- Sagemaker algorithm requires the input data in specific structured manner so to provide it in that way we create 4 folders('train', 'train_annotation', 'validation', 'validation_annotation').

- For semantic segmentation to work we need to create S3 bucket and upload the data on S3 bucket in specific manner.

- Then we create an instance of sagemaker estimator and pass the required parameters.

- After that, we plant the hyperparmeters.

- Before training process, we need to set the inputs for training job in same manner as we created bucket list folders.

- Now we launch the training job using instance of sagemaker estimator.(I got error here because of limitations of free AWS package)

- Now, we have to deploy this model now for predictions.

- After that we will plot the output image from our deployed model for an image from validation set(which was not used for training purpose).

- Now, we need to deleted the endpoints which were created during deployment of our model.

- For the last step, we need to shut our instance down or else AWS will charge a payment for overuse.

## Documentation

- [Amazon Sagemaker](https://docs.aws.amazon.com/sagemaker/index.html)

- [Boto3](https://boto3.amazonaws.com/v1/documentation/api/latest/index.html)

- [Pyplot](https://matplotlib.org/stable/api/_as_gen/matplotlib.pyplot.html)

- [Tqdm](https://tqdm.github.io/)

- [Tarfile](https://docs.python.org/3/library/tarfile.html)

- [Os](https://docs.python.org/3/library/os.html)

- [Shutil](https://docs.python.org/3/library/shutil.html)

- [Element tree](https://docs.python.org/3/library/xml.etree.elementtree.html)

- [Sagemaker estimator](https://sagemaker.readthedocs.io/en/stable/api/training/estimators.html)

- [Model Deployment](https://docs.aws.amazon.com/sagemaker/latest/dg/how-it-works-deployment.html)

## Acknowledgements

 - [Amit Yadav](https://www.coursera.org/instructor/amityadav)

## Feedback

If you have any feedback, please reach out to me at puranshu@iitg.ac.in.

## License

[MIT](https://choosealicense.com/licenses/mit/)

  
