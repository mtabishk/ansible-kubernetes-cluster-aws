# ansible-kubernetes-cluster-aws
Configure Kubernetes Cluster on AWS Cloud



https://user-images.githubusercontent.com/61789893/127108921-f21356bb-f8ea-4bc5-946e-fc3176de078a.mp4




### Step 1: Configure AWS CLI2 SDK
![0](https://user-images.githubusercontent.com/61789893/126860834-8f4bf522-0c1f-4cba-b6d4-6a185033701f.png)

### Step 2: Set some environmental variables
Replace with your aws credentials

![upd2](https://user-images.githubusercontent.com/61789893/126860849-2cdf5038-85d6-474f-a66b-269bdcf00b9d.png)

### Step 3: Update ansible.cfg file
Update the private_key_file with your AWS KeyPair

![an](https://user-images.githubusercontent.com/61789893/127128926-9726364b-303f-40d8-815d-c82343dd993e.png)

### Step 4: Update vars in launch_ec2_instances.yml file
Update keypair, image (Use AMI ID of Amazon Linux 2), vpc_subnet_id, security_group_id (SG should allow all ports), region, output_dir variables

![ee](https://user-images.githubusercontent.com/61789893/126861120-8d52f03f-4e77-4b5e-8f9d-45e35a3f331a.png)

![dd](https://user-images.githubusercontent.com/61789893/126861124-7c06530b-8c1d-4342-a2ce-38d98dc3cff6.png)

### Step 5: Run launch_ec2_instances.yml playbook
![2](https://user-images.githubusercontent.com/61789893/126861205-c85d1bad-f6d5-4e17-aade-ba1b7cae9773.png)

Check whether instances are launched in AWS Cloud.

![1](https://user-images.githubusercontent.com/61789893/126861226-8de7f399-851e-475c-a35b-d9d5f642dcce.png)


### Step 6: Run use_k8s_cluster_roles.yml playbook

![10](https://user-images.githubusercontent.com/61789893/127129134-cc69950f-529d-4071-b291-cb57cc62a3b9.png)

## Done!! 

### Now you can test your kubernetes cluster by running a deployment
![5](https://user-images.githubusercontent.com/61789893/126861535-015f8af5-8266-4272-8099-af6dd1705610.png)
![6](https://user-images.githubusercontent.com/61789893/126861540-3f29563f-b3df-42c2-b4dd-74af2ab02b8e.png)
![zz](https://user-images.githubusercontent.com/61789893/126861547-65957df8-a749-4ddc-ac47-ef873ce0a1ce.png)






