# Trusted Docker Image for MRI Ruby + Postgres client

## Use the Trusted Image

```
sudo docker run -i -t hopsoft/ruby-mri-postgres-client bash
ruby -v
```

## Build the Image Manually

#### Dependencies

* [Virtual Box](https://www.virtualbox.org/)
* [Vagrant](http://www.vagrantup.com/)

```
git clone https://github.com/hopsoft/docker-ruby-mri-postgres-client.git
cd docker-ruby-mri-postgres-client
vagrant up
vagrant ssh
sudo docker build -t hopsoft/ruby-mri-postgres-client /vagrant
```

Once the build finishes, you can [use the image](#use-the-trusted-image).

