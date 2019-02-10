### Download and Install PostgreSQL:
> docker run --name demo -e POSTGRES_PASSWORD=password1 -d postgres

### Verify Installation:
> docker exec -it demo psql -U postgres

Above command will launch the `psql tool` on the command line. Then run `\?` for help command.

 

