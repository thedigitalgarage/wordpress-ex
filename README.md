Scalable Wordpress in Digital Garage
------------------------------------

This git repository helps you configure and install Wordpress supporting scalability quickly. The plugins below are pre-configured:

* W3 Total Cache (https://wordpress.org/plugins/w3-total-cache/)
* Amazon Web Services (https://wordpress.org/plugins/amazon-web-services/)
* WP Offload S3 (https://wordpress.org/plugins/amazon-s3-and-cloudfront/)


Installation:
-------------------------

To install just make a fork this repository and use the oc to import the template and create the application:

```
$ oc create -f https://raw.githubusercontent.com/getupcloud/origin-templates/master/wordpress-template.yaml
$ oc new-app --template = wordpress-example --param = SOURCE_REPOSITORY_URL = http: //seu_repo/repo.git
```
Themes and Plugins
-------------------------

The themes and plugins must be copied to the appropriate directories on the local repository.

* wp-content / themes /
* wp-content / plugins /

Security
-------------------------

Check the Wordpress documentation for security best practices. Digital Garage automatically generates the secret keys in wp-config.php.
