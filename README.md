# Mahlwerk Tickets Push Card

## Deploying the Card

1. Clone the GitHub repository \ Download the zip and upload the file in BAS and extract it.
2. Deploy the Card.
3. Publish the Card.

## Creating a Push

1. Create a Service Key for register.
2. HTTP Method: POST
3. URL: Service URL `/mobileservices/origin/hcpms/CARDS/v1/register/templated`
4. Use the Alias as Username, and GUID as Passcode.
5. Add the following headers:
   * `Content-Type` - `application/json`
   * `Accept` - `application/json`
6. Add the following body:
   * ```json
        {
            "method": "REGISTER",
            "username": "p000253",
            "templateName": "Mahlwerk Push Ticket Card",
            "parameters": {
                            "ID1": "<Address ID>"
                        }
        }
