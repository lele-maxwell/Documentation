# Documentation
docs
>>># MULTIPASS DOCUMENTATION
Multipass is a tool to generate cloud-style Ubuntu VMs quickly on Linux, macOS and Windows. It provides a simple but powerful CLI that enables you to quickly access an Ubuntu command line or create your own local mini-cloud.
>>## In This Docummmention
- You will learn how to install and use multipass     
- You learn how to create an instance
- you will learn how to stop, purge, and delete instances runing on a virtual machine
>>### Install
- Run command `` snap install multipass ``
>>#### Use
- Run command `` multipass launch``
- Run the command `` multipass find `` to know the images availble
>>#### Creating an instance
- use ``multipass launch 22.04 --name docker-vm `` to create a new multipass instance based on the **Ubuntu 22.04**
image, and it assigns the name **docker-vm** to that instance. 
- use ``multipass shell docker-vm `` to manage and interact with your multipass instance directly from your terminal

>>#### Starting an instance
- use ``multipass start docker-vm`` to start the specific instance that has been previously created 
>>#### Stop an instance
- use ``multipass stop docker-vm`` to stop the specific instance 
>>#### Deleting an instance
- use `` multipass delete docker-vm `` to delete an instance
>>#### Purging an instance
- use `` multipass purge `` to delete all instances that have been marked for deletion
>>#### Aliasing 
This is used to create a shorter and easy to remember name of the instance. It is done by adding the  alias to the ``nano ~/.zshrc`` configuration file

- use ``multipass alias <alias-name> <instance-name>``
  in this case ``multipass alias one docker-vm`` the new alias name is ***one***


**_All these commands done on the comand line can be done_**  
**_using a ``PORTAINER`` which is the graphical user interface of a_** **``CONTAINER``** **_see_** [https://docs.portainer.io] **_for the documentation on portainers_** 
