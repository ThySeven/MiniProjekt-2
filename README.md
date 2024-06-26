# Welcome to MiniProjekt-2! 🚚

Welcome to our project repository! Here, you'll dive into the fascinating world of our delivery service and logistic control systems. Below, you'll find links to our repositories and a straightforward guide to get everything up and running.

## Project Repositories

- Delivery Service: [ThySeven/DeliveryService](https://github.com/ThySeven/DeliveryService)
- Planning Service: [ThySeven/PlanningService](https://github.com/ThySeven/PlanningService)
- Authorisation Service: [ThySeven/AuthService](https://github.com/ThySeven/AuthService)
- Tracking Service: [ThySeven/TrackingService](https://github.com/ThySeven/Tracking-Service)

## Getting Started

To get your environment set up and the services running smoothly, please follow these simple steps:

1. **Start the Common Services**  
   Begin by launching the common services needed for both the delivery and logistic aspects of the project. You can do so by executing the following command in your terminal:  
   `docker compose -f docker-compose-common.yml up -d`

2. **Initialize the Vault**  
   Next, set up the default Vault secrets. Simply run:  
   `docker compose -f docker-compose-vault-setup.yml up && docker compose -f docker-compose-vault-setup.yml down`
  
3. **Launch the Team Services**  
   To get the services for Team 1 and Team 2 up and running, use the command below, replacing `{id}` with `1` or `2` based on the team you're setting up for:  
   `docker compose -f docker-compose-team{id}.yml up -d`
  
   Alternatively:
   `docker compose -f docker-compose-team1.yml up -d && docker compose -f docker-compose-team2.yml up -d`

4. **???**  
   ???.

5. **Profit**  
   With everything set up, it's time to see your project come to life and enjoy the fruits of your labor!

Thank you for joining us on this exciting journey. Should you have any questions or need further assistance, feel free to reach out or check out our [GitHub issues](https://github.com/ThySeven/Miniprojekt-2/issues) section for support.

Happy coding! 🎉


## Dummy Data - Delivery

```json
{
    "id": "6098e6d7f0c35d30c4a07c93",
    "contact": {
        "name": "Emily",
        "address1": "555 Cedar Ave",
        "address2": "",
        "postalCode": 67890,
        "city": "Chicago",
        "contactName": "David Brown",
        "taxNumber": "135792468"
    },
    "address1": "777 Maple Rd",
    "address2": "Suite 100",
    "postalCode": 60611,
    "city": "Chicago",
    "deliveryDate": "2024-04-18T08:00:00Z"
}
