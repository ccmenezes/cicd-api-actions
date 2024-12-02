# CI-CD API Github Actions

This project was created to explore the build process using Github Actions, focused on the build stage and unit tests, to understand this stage in the pipeline context, increasing analytical thought as QAE Automation Tester.

## Getting Started

### Prerequisites
* Go (version 1.17 or newer recommended)
* Docker

### Steps to run locally

#### Using Docker

Using docker compose with simple commands you can start, check the logs, and shut down the application.

1. Start up the application.

```
docker compose -d
```
This command starts the application in the detached mod, making it possible to use the terminal still.

2. Check the logs.
```
docker compose logs -f
```
This command shows the logs for the application, both app and Postgres. To check them separately, add app or postgres after—f.


3. It's possible to check the API by any browser by localhost
```
http://localhost:8080/students
```

4. Finishing the application
```
docker compose down
```

5. Confirm the application was shot down
```
docker compose ls
```

#### Using Make

Only for unix-based users.

[make tutorial](https://www.computerhope.com/unix/umake.htm)

```
make build
```

The command make is responsible for running an existing stage at Makefile in this case we're running build, which represents the build process for the application.
These commands have the start, lint, and test stages.
Make is built Linux, then it's not necessary to any additional steps to install it.

## CI Execution

1. Automatic Triggers:
 - On push to main.
 - On pull request to main.

## Future Enhancements

1. Using secrets for sensitive data as password
2. Create a test coverage report


## Contribuitions
If you want to contribute to the project, from a developer, devOps or QA perspective, it will be a pleasure to accept your contribution.
