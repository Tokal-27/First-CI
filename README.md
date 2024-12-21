The Journey to Deployment

Once upon a time, a developer embarked on an exciting journey to bring an application to life. The steps of this adventure are chronicled below:

Chapter 1: The Code in the Vault

The first task was to safeguard the treasure—the Python application code. The developer pushed it to a private repository on GitHub, ensuring it was securely stored and ready for future use.

Chapter 2: Encasing the Treasure

To make the application portable and easy to deploy, the developer crafted a Dockerfile. This magical artifact containerized the application, making it ready to run anywhere. The Dockerfile was then committed and pushed to the GitHub repository.

Chapter 3: The Twin Machines

To test the deployment, the developer conjured two Vagrant machines. These humble machines, with low specifications, became the staging ground for the next steps in the adventure.

![Screenshot from 2024-12-20 14-19-53](https://github.com/user-attachments/assets/cbc78c41-cd6e-48cd-8d70-032f6a4828bf)![Screenshot from 2024-12-20 14-20-13](https://github.com/user-attachments/assets/82fbb9eb-33ac-43f7-85fd-355e496e883e)


Chapter 4: The Pipeline of Automation

The developer turned to Jenkins, a trusted ally, to automate the deployment process. The pipeline was set up to perform the following tasks:

Pull code from the Git repository (with the help of a credentials token):
Jenkins fetched the latest code, ensuring the pipeline always worked with the most up-to-date version.
![Screenshot from 2024-12-21 16-14-02](https://github.com/user-attachments/assets/70609e18-bd34-458e-9598-e8bfaaee2ca8)

Build a Docker image:
Jenkins built a Docker image from the application, encapsulating all dependencies and configurations.

Push the image to Docker Hub:

Chapter 5: The Ansible Magic

With the tools prepared, the developer used Ansible to perform the final tasks:

Installing Docker on the two target Vagrant machines:
Ansible ensured that Docker was installed and ready to use on both machines.

Pulling the Docker image from Docker Hub:
The image was retrieved from Docker Hub and brought to life on the Vagrant machines.

![Screenshot from 2024-12-21 18-41-36](https://github.com/user-attachments/assets/92595783-3840-4775-a2e7-0e38b9abc021)

Running a Docker container from the image:
Finally, the application was launched as a container, completing the journey.

![Screenshot from 2024-12-20 13-54-17](https://github.com/user-attachments/assets/7e1aa0eb-7282-41f1-9c94-de53955c642e)
![Screenshot from 2024-12-20 13-54-07](https://github.com/user-attachments/assets/adb984d3-e2be-4c86-8ad4-37a18bf4459b)
And so, the application was successfully deployed, marking the end of this thrilling adventure—for now. Every step taken was a testament to the power of automation, containerization, and collaboration.

