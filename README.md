# spring-gumball ci/cd example
# spring-gumball

Part 1 - CI workflow</br>

1. CI workflow </br>
A push is made to the main branch on git trigger the gradle workflow which build the jar file every a push is made. </br>
![lab10Image1-CI](https://github.com/ShanShanLee3/spring-gumball/blob/main/images/lab10Image1-CI.png) <br/>

Part 2 - CD workflow</br>

2. GCP Service Account </br>
A service account is made on google cloud platform </br>
![lab10Image2-SA](https://github.com/ShanShanLee3/spring-gumball/blob/main/images/lab10Image2-SA.png) <br/>

3. GCP Service Account Key </br>
A key is generated for the service account </br>
![lab10Image3-SA-key](https://github.com/ShanShanLee3/spring-gumball/blob/main/images/lab10Image3-SA-key.png) <br/>

4. Github secrets key </br>
The service account key generated is stored in the github setting. </br>
![lab10Image3A-secrets](https://github.com/ShanShanLee3/spring-gumball/blob/main/images/lab10Image3A-secrets.png) <br/>

5. First Release v1.0 </br>
The first release is made to trigger the workflow to deploy on GKE, but this release is failed due to error credentials. </br>
![lab10Image4-release1](https://github.com/ShanShanLee3/spring-gumball/blob/main/images/lab10Image4-release1.png) <br/>

6. Third Release v1.2 </br>
After several release attempts, a release is made successfully. </br>
![lab10Image5-release3](https://github.com/ShanShanLee3/spring-gumball/blob/main/images/lab10Image5-release3.png) <br/>

7. Versions </br>
All the pushes and releases are recorded on github under actions. </br>
![lab10Image6-v](https://github.com/ShanShanLee3/spring-gumball/blob/main/images/lab10Image6-v.png) <br/>

8. Deployment </br>
After a release is successful, the image is deployed to GKE. </br>
![lab10Image7-deployment](https://github.com/ShanShanLee3/spring-gumball/blob/main/images/lab10Image7-deployment.png) <br/>

9. Service </br>
![lab10Image8-service](https://github.com/ShanShanLee3/spring-gumball/blob/main/images/lab10Image8-service.png) <br/>

10. Ingress </br>
Creating a load balancer manually for the UI. </br>
![lab10Image9-ingress](https://github.com/ShanShanLee3/spring-gumball/blob/main/images/lab10Image9-ingress.png) <br/>

11. Load Balancer </br>
The load balancer is up. </br>
![lab10Image10-lb](https://github.com/ShanShanLee3/spring-gumball/blob/main/images/lab10Image10-lb.png) <br/>

12. Spring-gumball on GKE </br>
The Spring-gumball UI is viewable from load balancer. </br>
![llab10Image11-UI](https://github.com/ShanShanLee3/spring-gumball/blob/main/images/lab10Image11-UI.png) <br/>