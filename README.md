# DEMO: Simple OAuth2 Authorization Server 
This project demonstartes how to create a very simple Authorization Server using Spring Boot 2, Spring Security and Spring OAuth2.

## @EnableAuthorizationServer
This annotation is used to configure the OAuth 2.0 Authorization Servermechanism.

## Tokens Generation
By default, access_token and refresh_token are being generated via random value. This is taken care by framework class DefaultTokenServices.

## InMemoryTokenStore
DefaultTokenServices delegates persistence of tokens to TokenStore. The default store is in-memory implementation: InMemoryTokenStore.

## How to Switch On Password Grant

### Step-1: Add the below code snippet in your Web Security COnfiguration.

```bash
    @Override
    @Bean
    public AuthenticationManager authenticationManagerBean() throws Exception {
       return super.authenticationManagerBean();
    }
```

