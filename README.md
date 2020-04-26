# aws-lambda-chaos-monkey
an aws lambda function to terminate a random EC2 instance in your environment.
this function is used for stability testing of your envirenment.
Be carefull it might terminate an instance you don't need to terminate it.

# How to use it 
1- npm install<br>
2-run :  zip -r chaos-monkey.zip .   // to create a zip file of your function <br>
3- in your aws console create a lambda function and associate to it the policies:<br> -EC2 Describe instances and EC2 terminate instances<br>
4- attach it to cloud watch if you want to run this instance periodically<br>
