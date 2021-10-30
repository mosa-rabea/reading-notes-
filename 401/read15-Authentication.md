# Spring Security Architecture
Application security boils down to two more or less independent problems: authentication (who are you?) and authorization (what are you allowed to do?).



## Authorization 
Once authentication is successful,
we can move on to authorization,
and the core strategy here is AccessDecisionManager. 

An AccessDecisionVoter considers an Authentication (representing a principal) and a secure Object
, which has been decorated with ConfigAttributes:

```
boolean supports(ConfigAttribute attribute);

boolean supports(Class<?> clazz);

int vote(Authentication authentication, S object,
        Collection<ConfigAttribute> attributes);
```

### Web Security
* Spring Security in the web tier (for UIs and HTTP back ends) is based on Servlet Filters .

* The client sends a request to the application, and the container decides which filters and which servlet apply to it based on the path of the request URI.

* Spring Security is installed as a single Filter in the chain, and its concrete type is FilterChainProxy.

* the security filter is a @Bean in the ApplicationContext, and it is installed by default so that it is applied to every request.

* There can be multiple filter chains all managed by Spring Security in the same top level FilterChainProxy and all are unknown to the container.










