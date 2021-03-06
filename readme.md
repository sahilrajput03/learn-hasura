# README

TODO: Hasura Actions in Action with its Co-Founder Tanmai Gopal aka @tanmaigo: [Click here](https://youtu.be/KH3mv4tm0fY?list=LL)

Learn hasura Page on Github Profile: [Click here](https://github.com/sahilrajput03/sahilrajput03/blob/master/learn-hasura.md)

Hasura Graphql Engine: [Click here](https://github.com/hasura/graphql-engine)

- in a new directory run `wget https://raw.githubusercontent.com/hasura/graphql-engine/stable/install-manifests/docker-compose/docker-compose.yaml`
- `docker-compose up -d` or `dc up -d`
- `docker ps` or `dk ps`
- Connection link for postgres db: [click here](https://github.com/sahilrajput03/learning_sql/blob/main/Notes_setup-postgres.md#hasura-connecting-db)

FYI: To turn down use, `dc down` command.

tldr: 

```txt
- Database Display Name: `myDb1_blogs_test`
- Database URL: `postgresql://postgres:secret@192.168.18.3:5432/myDb1_blogs_test` or `postgresql://postgres:secret@192.168.18.3:5432/myDb1_test`
```

##### Setting up local postgres for hasura

[Click here](https://github.com/sahilrajput03/learning_sql/blob/main/Notes_setup-postgres.md#hasura-connecting-db)

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

- View table's data: 

![image](https://user-images.githubusercontent.com/31458531/177782803-d90183b7-0da6-42f0-9b18-0c86c995a98c.png)

- Insert row in a table: 

![image](https://user-images.githubusercontent.com/31458531/177783002-901f5e9c-2b7d-41aa-adad-2ee1593288b6.png)

- Copy request code via ***Code Exporter***: 

![image](https://user-images.githubusercontent.com/31458531/177784758-83de7ff0-a777-45de-af88-154f8136db38.png)

- You can analyse the sql query generated by the gql query you have written:

![image](https://user-images.githubusercontent.com/31458531/177806490-7c091126-b7a8-4334-ab50-a89652531d9f.png)

![image](https://user-images.githubusercontent.com/31458531/177806390-fca7163d-7204-48ad-a44a-e56a28fc813d.png)

- Making mutation: 

![image](https://user-images.githubusercontent.com/31458531/177827118-016c8505-87c6-47fb-acc0-aa05b519ca45.png)

- Adding default value for `created_at` and `updated_at` so that they take values on their own when the query is sent without those values: 

![image](https://user-images.githubusercontent.com/31458531/177828240-62c6445c-3f8d-4b4e-a4f3-ab8c68e88e54.png)

![image](https://user-images.githubusercontent.com/31458531/177828526-3ade2c9a-09e3-4268-b132-94c3f6a481ea.png)

- We can make combined queries, also i am using aggregate query to calculate number of blogs as well:

![image](https://user-images.githubusercontent.com/31458531/177960510-f56c2512-0c8e-417e-bec4-d945f8798a55.png)

- Protect you hasural panel with a password [in docs](https://hasura.io/docs/latest/graphql/core/deployment/graphql-engine-flags/config-examples/):

![image](https://user-images.githubusercontent.com/31458531/178027106-1c938da5-6067-4440-be6e-441823d80401.png)

and then webpage would look like this -

![image](https://user-images.githubusercontent.com/31458531/178027510-0ae23ae6-dd90-436d-b6e9-f3704d574d2c.png)
