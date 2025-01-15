# Description
Show me how to develop an application to allow customers to see a list of dogs to adopt in their area similar to a dating app like Bumble.

# User types
Admin - A user who manages the data
Adopter - A user who intends to see animals in the area to adopt
Adoptee - A user who intends to post and animal for adoption
[Note: An adopter may post an animal for adoption or an adoptee may adopt animal]

# Requirements
- Users must be able to register with Google, Apple ID or Facebook.
  - Upon registering, they must choose if they wish to adopt or post animals to adopt.
- Adopters must answer a simple list of questions to understand their preference in animal.  
  - Cat or Dog
  - Animal size (Large, Medium, Small)
  - Fur Type (Furry, not Furry, hypoallergenic, No preference)
  - What breed [Optional]
  - Age (Young, Adult, Senior)
- After answering the questionnaire, the adopter must start to see animals in their area
  - For future logins, animal swiping will immediately appear
- An Adopter will see a Picture of the animal with their name and age.
- An adopter can select the X button  to go to the next animal
- An adopter can select the Check button to start a chat with the adoptee
- An adopter can swipe right to start a chat with the adoptee
- An adopter can click on an animal to see profile info
- After registering, the adoptee option must be disabled for future development
- An adopter can click a profile icon at the top right to access profile settings or log out
- A user can modify their name and adopter preferences in the profile settings

# System Architecture
- C# .NET Minimal API microservices backend
- SQL database backend
- React frontend which references APIs for all data access
- RabbitMQ to handle events
- Redis to handle caching
- Google analytics for site access
- Logging must be stored with Sentry.io
- Use .NET for Gateway

# Application design
- APIs must follow clean architecture
- Use design patterns to minimize coupling
- Use Entity Framework as an ORM
- Database must be code first using EF migrations
- Microservices must use XUnit for unit testing
- React must use unit testing
- React must use Material UI (MUI) for a minimalist simple light UI

# Coding Standards
- Make sure all class, method and variable names are descriptive
- All configurable information must be stored in configuration files
- Follow SOLID principles

# Data
- Follow normalization standards for SQL database schema
- Minimize hard types for animals to allow for easy extensions in the future

# Hosting
- Github repository
- Azure AKS for fully containerized solution
- Docker for local hosting
- Kubernetes for orchestration
- Azure blob storage for images
- Deploy with Github Actions