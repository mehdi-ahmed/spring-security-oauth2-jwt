- Source: https://www.danvega.dev/blog/spring-security-jwt
# Spring Security JWT
  - Spring Security has built-in support for JWTs using oAuth2 Resource Server. In this tutorial you are going to learn how to secure 
    your APIs using JSON Web Tokens (JWT) with Spring Security.

# Topics covered
- Config class with securityFilterChain that enables authenticated users
- creation of an InMemoryUser with password encryption {noop}
- public/private key generation - Externalization with @ConfigurationProperties and config file
- @EnableConfigurationProperties(RsaKeyProperties.class) and @ConfigurationProperties(prefix = "rsa")
- jwtEncoder(), jwtDecoder()
- TokenService with generateToken, expireDate
- IT Test with @WebMvcTest( -- controllers - ) and @Import({SecurityConfig.class, TokenService.class})
- @Autowired MockMvc in test