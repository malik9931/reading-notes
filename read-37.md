What is Amazon S3?

Amazon Simple Storage Service (Amazon S3) - is storage for the Internet.
 

Advantages of using Amazon S3
Creaing buckets
Storing data
Downloading data
Permissions
Standard interfaces
 

Amazon S3 features
Storage classes - Amazon S3 offers a range of storage classes designed for different use cases.
Bucket policies - provide centralized access control to buckets and objects based on a variety of conditions, including Amazon S3 operations, requesters, resources, and aspects of the request. Are expressed in the access policy language and enable centralized management of permissions. The permissions attached to a bucket apply to all of the bucket's objects that are owned by the bucket owner account.
Amplify Storage

Amplify Storage category - provides an interface for managing user content for your app in public, protected, or private storage buckets.
Setup
Provision backend storage - execute the command: amplify add storage, and then answer the questions
To push changes to the cloud use the command: amplify push
Install Amplify Libraries - add these dependencies { implementation 'com.amplifyframework:aws-storage-s3:1.17.1' implementation 'com.amplifyframework:aws-auth-cognito:1.17.1' }
Initialize Amplify Storage - initialize the Amplify Auth and Storage categories you call Amplify.addPlugin() method for each category. To complete initialization call Amplify.configure(). Add the following code: Amplify.addPlugin(new AWSCognitoAuthPlugin()); Amplify.addPlugin(new AWSS3StoragePlugin());
Uploading data to your bucket - specify the key and the data object to be uploaded.
Upon successfully executing this code, you should see a new folder in your bucket, called public. It should contain a file called ExampleKey, whose contents is Example file contents.
