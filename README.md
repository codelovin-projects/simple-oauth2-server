# DEMO: Simple OAuth2 Authorization Server 
This project demonstartes how to create a very simple Authorization Server using Spring Boot 2, Spring Security and Spring OAuth2.

## @EnableAuthorizationServer
This annotation is used to configure the OAuth 2.0 Authorization Servermechanism.

## Tokens Generation
By default, access_token and refresh_token are being generated via random value. This is taken care by framework class DefaultTokenServices.
