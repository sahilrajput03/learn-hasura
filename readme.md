# README

Learn hasura Page: [Click here](https://github.com/sahilrajput03/sahilrajput03/blob/master/learn-hasura.md)

Hasura Graphql Engine: [Click here](https://github.com/hasura/graphql-engine)

- in a new directory run `wget https://raw.githubusercontent.com/hasura/graphql-engine/stable/install-manifests/docker-compose/docker-compose.yaml`
- `docker-compose up -d`
- `docker ps`
- Connection link for postgres db: [click here](https://github.com/sahilrajput03/learning_sql/blob/main/Notes_setup-postgres.md#hasura-connecting-db)

tldr: 

```txt
- Database Display Name: `myDb1_blogs_test`
- Database URL: `postgresql://postgres:secret@192.168.18.3:5432/myDb1_blogs_test` or `postgresql://postgres:secret@192.168.18.3:5432/myDb1_test`
```

## Resources

- Getting Started Docs: [Click here](https://hasura.io/docs/latest/graphql/core/getting-started/first-graphql-query/#create-a-table)
- Hasura - Getting Started (Your First Query) : [Click here](https://youtu.be/ZGKQ0U18USU)
- Official Course by Hasura: [Click here](https://hasura.io/learn/graphql/hasura/introduction/?pg=oss-console&plcmt=onboarding-checklist)

## Pictorial Memory

- Connecting to local db say `myDb1_blogs_test`:

![image](https://user-images.githubusercontent.com/31458531/177777669-66ea22e2-6535-41bc-997e-0ced5d06024e.png)

- Now view the database: 

![image](https://user-images.githubusercontent.com/31458531/177777934-23a6b256-cd69-49fc-af8e-c4551f1ad854.png)

- Now track some tables: 

![image](https://user-images.githubusercontent.com/31458531/177778852-dd8cf5a6-2fa6-400b-bc9c-6c6de2910c83.png)


- Now you can make use of graphql queries - Example of making use of an aggregate query where we can limit the number of items, provide offset, provide the required fields, order by using any combination of sequelize operators like `eq`, `or` like operators. Yikes!!

![image](https://user-images.githubusercontent.com/31458531/177779920-2db69b4a-6270-41a3-83f2-55a6bbcf9450.png)
