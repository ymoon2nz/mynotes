Snowflake Security
--------


# Role Model

```
create user user1 
  PASSWORD = 'password1'
;
create user user1 
  PASSWORD = 'password1'
;

create schema schema1;
create role r_schema1_ro;
create role r_schema1_rw;
create role r_schema1_own;

create table schema1.tab1 (col1 int, col2 varchar(100));

grant usage on schema schema1 to role r_schema1_ro;
grant usage on schema schema1 to role r_schema1_rw;
grant owership on schema schema1 to role r_schema1_own;


```