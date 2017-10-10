# CORS through Content Security Policy

Use to be enabled via meta tags but is now best practice to enable via server headers. Enables CORS to google domain.

## Example with header
```
Content-Security-Policy:default-src 'self';script-src 'self' 'unsafe-inline' 'unsafe-eval' https://www.google.com; 
```

## Example with metatags (not recommended as can be altered)
```
<meta http-equiv="Content-Security-Policy" content="default-src https://www.google.com">
```
