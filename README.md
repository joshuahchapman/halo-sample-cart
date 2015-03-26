# E-commerce Cart Sample

The cart sample includes a Vagrantfile, behat tests and plain old PHP objects (POPOs) that model the functionality of a basic shopping cart.

## Requirements

The cart sample uses Vagrant to provision and configure a Virtual Machine that satisfies all the dependencies for the code to work.

   * VirtualBox 4.3.18 (or higher). Download here: https://www.virtualbox.org/wiki/Downloads
   * Vagrant 1.7.2 (or higher). Download here: http://www.vagrantup.com/downloads

## Installation

   * Make sure you have a working internet connection. The virtual machine will be downloading packages from the internet in order to configure itself.
   * Start the Vagrant box (VM) by typing: `vagrant up`
   * During the startup process, the virtual machine will be provisioned with git, php and composer.

## Running Tests

After installation, ssh into the vagrant box and confirm the tests are working:

```bash
$ vagrant ssh
$ cd /vagrant
$ behat
```

The tests should complete without errors. The majority of the tests will be in a pending state.

## Code Layout

Here is a high level overview of the important files in this project:

   * `features/cart.feature` - the gherkin language that describes scenarios (tests cases) for the sample cart code.
   * `features/bootstrap/FeatureContext.php` - the Behat file that parses the above `cart.feature` and executes tests.
   * `src/HauteLook/Cart.php` - the sample cart class
   * `src/HauteLook/Product.php` - the same product class

Vagrant will automatically sync any changes made to these files. Feel free to use whatever editor you are most comfortable with to browse and edit these files.

## Challenge

The first scenario has been written for you. Please implement as many of the remaining scenarios in `features/cart.feature` as you can within the next 60 minutes. Do not worry if you cannot finish all of them. Find a good stopping point and send us what you have. We are excited to see it! Zip up the entire directory and email it back to us.

### Support

Need help? Please reach out to us! We know computers can be tricky things and we are happy to assist you. You should have contact details from our email to you. We will get back to you as soon as we can.


