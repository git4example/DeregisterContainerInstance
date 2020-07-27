# DeregisterContainerInstance

### How to Use :

This python script will accept the input as container instanceId(not ec2 instanceID) and the cluster name. 

    $ python deregisterContainerInstance.py -i <Container-Instance-Id> -c <ECS-Cluster-Name>

### What it do : 
    1. Get all the tasks from the container instance.
    2. Set the container instance state to "DRAINING" state.
    3. Stop all the tasks on the container instance.
    4. De-Register the container instance from the appropriate cluster

