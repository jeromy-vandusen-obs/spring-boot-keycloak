# Simple UI for OAuth2 Integration with Keycloak Sample Application

## Environment Variables

* KEYCLOAK_URL: The URL of the Keycloak server (default is `http://keycloak.rarysoft.local`).
* KEYCLOAK_REALM: The Realm defined in the Keycloak server (default is `rarysoft`).
* KEYCLOAK_CLIENT: The Client ID defined in the Keycloak server (default is `rarysoft-sample`).
* KEYCLOAK_CLIENT_IS_PUBLIC: Whether or not the Client is public (default is `true`).

## Keycloak Configuration

In Keycloak, create a realm. Plug the realm name into the KEYCLOAK_REALM environment variable. Create a client. Plug
the client ID into the KEYCLOAK_CLIENT environment variable. Create a role called `user`. Create a user and assign the
`user` role to the new user. If a different role name is preferred, modify the `SecurityConfiguration` class in the
`com.rarysoft.simpleui.security` package and set the preferred role name in the `configure(HttpSecurity http)`
method.
