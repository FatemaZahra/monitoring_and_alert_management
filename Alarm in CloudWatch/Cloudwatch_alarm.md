### Steps to create an Alarm on CloudWatch

1. Go to CloudWatch Service --> Click on Create Alarm

![Screenshot 2022-08-26 at 12 14 05](https://user-images.githubusercontent.com/102330725/186893195-c97635e3-438b-4d64-9e7f-c6a73ed47ba1.png)

2. Search for the instance for which the alarm is to be set.

![Screenshot 2022-08-26 at 12 14 51](https://user-images.githubusercontent.com/102330725/186893551-c83b5dcf-c477-4ea8-b46b-ee06fe18bc6c.png)

3. When the instance pops-up select EC2 > Per-Instance Metrics.

![Screenshot 2022-08-26 at 12 15 03](https://user-images.githubusercontent.com/102330725/186893784-8727a6df-1fea-4dae-9f13-ebf12b112f38.png)

4. Select the metric for which the alarm is to be set from the list.

![Screenshot 2022-08-26 at 12 15 18](https://user-images.githubusercontent.com/102330725/186941527-fb713b52-b9c8-40fd-b575-24042af12add.png)

5. Once the metric is selected, the page to specify metric and conditions opens up

![Screenshot 2022-08-26 at 12 16 13](https://user-images.githubusercontent.com/102330725/186941694-7723b15f-1c0d-4585-bd76-345d6939147f.png)

6. Add the conditions and move to next

![Screenshot 2022-08-26 at 12 16 34](https://user-images.githubusercontent.com/102330725/186943565-e6fdde23-4766-4c21-94a6-2efa36db56bb.png)

7. Under configure actions, Create a new Topic and add a name as well as an email ID to receive SNS notifications and move to next

![Screenshot 2022-08-26 at 12 16 49](https://user-images.githubusercontent.com/102330725/186943740-76a50bbc-ab32-4ba0-8cfb-ae76b0b906a7.png)

8. Provide a name and description for the alarm

![Screenshot 2022-08-26 at 12 20 57](https://user-images.githubusercontent.com/102330725/186944664-5ab66f90-f368-47ff-b39e-926ebf217889.png)

9. Preview the details added and create the alarm

![Screenshot 2022-08-26 at 12 21 12](https://user-images.githubusercontent.com/102330725/186944742-7e942014-7dc8-4202-9f68-118c12c88e5c.png)
