# RegexCheatSheet

## Password validation

Minimum 8 characters, at least one letter and one number
```
^(?=.*[A-Za-z])(?=.*\d)[A-Za-z\d]{8,}$
```

Minimum 8 characters, at least one letter, one number and one special character
```
^(?=.*[A-Za-z])(?=.*\d)(?=.*[@$!%*#?&])[A-Za-z\d@$!%*#?&]{8,}$
```

Minimum 8 characters, at least one uppercase letter, one lowercase letter and one number

```
^(?=.*[a-z])(?=.*[A-Z])(?=.*\d)[a-zA-Z\d]{8,}$
```

Minimum 8 characters, at least one uppercase letter, one lowercase letter, one number and one special character
```
^(?=.*?[A-Z])(?=.*?[a-z])(?=.*?[0-9])(?=.*?[#?!@$%^&*-]).{8,}$
```

Minimum 8 and maximum 10 characters, at least one uppercase letter, one lowercase letter, one number and one special character
```
^(?=.*[a-z])(?=.*[A-Z])(?=.*\d)(?=.*[@$!%*?&])[A-Za-z\d@$!%*?&]{8,10}$
```

## References
https://stackoverflow.com/questions/19605150/regex-for-password-must-contain-at-least-eight-characters-at-least-one-number-a
