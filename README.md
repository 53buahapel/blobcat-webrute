# Login Page Bruteforce Tools

## Description

This is a simple tool to bruteforce login pages. It is written in Python and uses the requests library to send HTTP requests.

## Simple Usage

```ps
python3 main.py --url URL --data DATA --wordlist WORDLIST --expected EXPECTED

# example

python3 main.py --url http://example.com/login --data "username=admin&password=*" --wordlist wordlist.txt --expected "Invalid username or password"
```

## Options

- `--url` - The URL of the login page
- `--data` - The POST data to send to the login page. You can use the `*` character to replace with the wordlist value
- `--ctype` - The content type of the POST data. Choose 0 for `x-www-form-urlencoded` and 1 for `JSON`
- `--wordlist` - The location of the wordlist file
- `--expected` - The expected response when the login fails
- `--threads` - The number of threads to use
- `--random-agent` - Use a random user agent

## Contributing

Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.