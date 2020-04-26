# aws-lambda-chaos-monkey
an aws lambda function to terminate a random EC2 instance in your environment.
this function is used for stability testing of your environment.
Be careful it might terminate an instance you don't need to terminate it.

# How to use it 
<ol>
<li>npm install</li>
<li>run :  <code>zip -r chaos-monkey.zip . </code>  <comment>to create a zip file of your function</comment>  </li>
<li> in your aws console create a lambda function and associate to it the policies:<br> -EC2 Describe instances and EC2 terminate instances</li>
<li> upload your zip file</li>
<li> attach it to cloud watch if you want to run this instance periodically</li>
</ol>
