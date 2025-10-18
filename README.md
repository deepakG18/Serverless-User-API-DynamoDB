
# Serverless User Management API

A production-ready serverless REST API built with AWS Lambda, DynamoDB, and API Gateway for managing user data with full CRUD operations.

## 🚀 Features

- **Full CRUD Operations**: Create, Read, Update, and Delete user records
- **Serverless Architecture**: Zero server management using AWS Lambda
- **Scalable NoSQL Database**: DynamoDB for high-performance data storage
- **RESTful API**: Clean API Gateway endpoints with proper HTTP methods
- **CI/CD Pipeline**: Automated deployment using GitHub Actions
- **Monitoring & Logging**: CloudWatch integration for debugging and monitoring
- **IAM Security**: Granular permissions per Lambda function for enhanced security

## 🛠️ Tech Stack

- **Runtime**: Node.js 14.x
- **Cloud Provider**: AWS (Lambda, DynamoDB, API Gateway)
- **Framework**: Serverless Framework
- **CI/CD**: GitHub Actions
- **Monitoring**: AWS CloudWatch
- **Infrastructure**: Infrastructure as Code (IaC)

## 📌 API Endpoints

| Method | Endpoint | Description |
|--------|----------|-------------|
| POST | `/post` | Create a new user record |
| GET | `/posts` | Retrieve all user records |
| GET | `/post/{postId}` | Retrieve a specific user by ID |
| PUT | `/post/{postId}` | Update an existing user record |
| DELETE | `/post/{postId}` | Delete a user record |

## 🏗️ Architecture

Client Request
↓
API Gateway (RESTful endpoints)
↓
AWS Lambda Functions (Node.js)
↓
DynamoDB Table (NoSQL Database)
↓
CloudWatch Logs (Monitoring)


### Key Components:
- **API Gateway**: Routes HTTP requests to appropriate Lambda functions
- **Lambda Functions**: Execute business logic with IAM role permissions
- **DynamoDB**: Stores user data with partition key-based access
- **CloudWatch**: Logs execution details for debugging

## 📦 Project Structure

├── api.js # Lambda function handlers
├── serverless.yml # Serverless Framework configuration
├── package.json # Node.js dependencies
├── .github/
│ └── workflows/
│ └── main.yml # CI/CD pipeline configuration
└── README.md # Project documentation


## 🚀 Deployment

This project uses **GitHub Actions** for automated deployment to AWS.

### Prerequisites:
- AWS Account with programmatic access
- GitHub repository with AWS credentials configured as secrets

### Deployment Steps:
1. Push code to the `main` branch
2. GitHub Actions automatically triggers deployment
3. Serverless Framework packages and deploys to AWS
4. API Gateway endpoint is created and available for use

## 🔐 Security

- **IAM Roles**: Each Lambda function has granular permissions (least privilege principle)
- **Environment Variables**: Sensitive data stored securely
- **No Hardcoded Credentials**: All access managed through AWS IAM

## 📊 Monitoring

CloudWatch Logs track:
- Lambda function execution times
- Error rates and debugging information
- Request/response patterns
- DynamoDB read/write operations

## 👨‍💻 Author

**Deepak Gupta**  
B.Tech Electrical Engineering | DevOps & Cloud Engineering Enthusiast

🔗 [GitHub](https://github.com/deepakG18) | [LinkedIn](https://www.linkedin.com/in/deepak-gupta-910775288)

## 📝 License

This project is open source and available for learning purposes.


