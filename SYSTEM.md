# Description
A modern webapp to allow pet adopters to interact with adoptable animals in their area similar to a dating app like Bumble.

# User types
Admin - A user who manages the data
Adopter - A user who intends to see animals in the area to adopt
Adoptee - A user who intends to post and animal for adoption
[Note: An adopter may post an animal for adoption or an adoptee may adopt animal]

# Requirements
- Users must be able to register with Google, Apple ID or Facebook.
  - Upon registering, they must choose if they wish to adopt or post animals to adopt.
- An adopter must answer a simple list of questions to understand their preference in animal.  
- After answering the questionnaire, the adopter must start to see animals in their area
- An adopter will see a Picture of the animal with their name and age.
- An adopter can select the X button  to go to the next animal
- An adopter can select the Check button to start a chat with the adoptee
- An adopter may optionally send payment to adoptees
- An adopter may send donations to adoptees
- After registering, the adoptee option must be disabled for future development
- An adopter may click a profile icon at the top right to access profile settings or log out
- A user may modify their name and adopter preferences in the profile settings
- An adoptee may list a new animal with a basic profile for a small fee
- A user may access their chats at anytime
- An adoptee may update or remove their animal listing at anytime

# AI Agent Integration
- Image submission moderation agent
- Animal or user profile moderation agent
- Profile assistant agent
- Email support agent

# Income streams
- Animal listing fees
- Adopter to Adoptee transaction fees
- Adopter animal adoption fees
- 
# System Architecture
- C# .NET Minimal API microservices backend
- SQL database backend
- React frontend which references APIs for all data access
- RabbitMQ to handle events
- Redis to handle caching
- Google analytics for site access data
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
