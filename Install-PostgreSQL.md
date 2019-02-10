### Download and Install PostgreSQL:
> docker run --name demo -e POSTGRES_PASSWORD=password1 -d postgres

### Verify Installation:
> docker exec -it demo psql -U postgres

Above command will launch the `psql tool` on the command line. Then run `\?` for help command.

 ![](https://github.com/manas86/postgres-tutorial/blob/master/help-command.png)

In another window you can type `docker ps` to check and verify if above container is running
