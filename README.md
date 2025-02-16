# DevOps Web App

## Overview
This is a DevOps-powered web application designed to demonstrate best practices in CI/CD and cloud deployment using AWS. The project integrates automation, monitoring, and scalability to showcase a modern web application lifecycle.

## Features
- **Java Web Application**: Built using Java and Maven
- **CI/CD Pipeline**: Automated builds, testing, and deployment
- **AWS Integration**: Hosted on an EC2 instance with SSH access
- **Infrastructure as Code (IaC)**: AWS CloudFormation for infrastructure management
- **Monitoring & Logging**: Integrated logging and performance monitoring
- **Security Best Practices**: Secure configurations and vulnerability scanning

## Technologies Used
- **Programming Language**: Java
- **Build Tool**: Maven
- **Cloud Platform**: AWS (EC2 instance for deployment)
- **CI/CD Tools**: GitHub Actions
- **Infrastructure as Code**: AWS CloudFormation
- **Monitoring & Logging**: AWS CloudWatch


## Getting Started
### Prerequisites
Ensure you have the following installed:
- Java (Installed on EC2 instance)
- Maven (Installed on EC2 instance)
- SSH Access to EC2
- Git (Configured to push changes to remote repo)
- AWS CLI (Configured for CloudFormation management)

### Installation & Setup
1. **Clone the Repository:**
   ```sh
   git clone https://github.com/abhishekbhagat98/devops-webapp.git
   cd devops-webapp
   ```
2. **Connect to EC2 Instance via SSH:**
   ```sh
   ssh -i your-key.pem ec2-user@your-ec2-ip
   ```
3. **Set Up Environment Variables:**
   ```sh
   cp .env.example .env
   # Update the .env file with appropriate values
   ```
4. **Build & Run the Application on EC2:**
   ```sh
   mvn clean install
   java -jar target/your-app.jar
   ```
5. **Deploy Infrastructure using AWS CloudFormation:**
   ```sh
   aws cloudformation deploy --template-file cloudformation.yml --stack-name my-stack
   ```
6. **Access the Application:**
   Open `http://your-ec2-ip:port` or the configured domain.

## CI/CD Workflow
The repository includes a CI/CD pipeline that:
- Runs automated tests on every push
- Deploys the application to an AWS EC2 instance
- Manages infrastructure using AWS CloudFormation

## Contributing
Contributions are welcome! Follow these steps:
1. Fork the repository
2. Create a new branch (`feature-branch`)
3. Commit changes and push to your fork
4. Submit a pull request

## License
This project is licensed under the MIT License. See `LICENSE` for details.

## Contact
For queries or collaborations, reach out via LinkedIn.

