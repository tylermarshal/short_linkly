# Short Linkly

## Welcome to Short Linkly a link shortening service!

Built with Rails 5.2.3 and Ruby 2.5.1

This app is an unfinished URL shortening service, similar to bit.ly. For the first deliverable, a completed test suite has been written out for you. Please do not change any existing tests; you will need to write your code in order to get them to pass.

- Implement unique shortened URLs for users.
- All short links require a unique long link and user_id.
- Here is an example request to your service:

```
POST http://localhost:8080/short_link
{
  "long_url": "<long_url>",
  "user_id": "<user_id>"
}
```
- If the long_url has already been shortened for a user, you should return the previously created short_link. Otherwise, you should return a new short_link. The response should look something like:

```
{
  "long_url": "<long_url>",
  "short_link": "<short_link>"
}
```

For the second deliverable, a test suite has not been previously written.

- Implement an analytics endpoint, which takes an encoded id and renders the short link, the long link, and the number of times the short link has been accessed.
- Please use the following URI pattern: `/:id/analytics`

You will have 2 hours to complete this project. Err on the side of completeness of individual features, over completing all features. You can use any tools you'd like. Thanks in advance for taking the time do do this exercise!

## Setup

```shell
bundle install
```

### postgresql

If you have not already install postgresql

```shell
brew install postgresql
```

and start postgresql

```shell
brew services start postgresql
```

### Create Databse

```shell
rails db:create db:migrate
```

### Start Rails Server

```shell
rails s
```

