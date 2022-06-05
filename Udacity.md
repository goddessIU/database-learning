# chapter2
## database schema
类似于是数据库的结构、定义
student(ID, name, phone) 算是schema， 就是数据库的attribute和他们的domain

## database instances
数据库的快照

relation如果是变量，schema是变量的类型和定义，instance是值

## keys
### superkey
superkey可以区别出不同的tuple， 如果id可以区别出，id+name也是superkey， name是无关的

### candidate key
这个superkey子集不是superkey，就是candidate key

### primary key

### foreign key
该属性是另一个relation的primary key

## relational algebra(P53)
selection \ projection \ natural join \ cartesian product \ union 


# chapter3
## SQL 
### parts of SQL
1. data-definition language DDL: define relation schemas, deleting relations and modifying relation schemas
2. data-manipulation language(DML):数据增删改查
3. Integrity
4. view definition
5. transaction control
6. embedded sql and dynamic sql
7. authorization

## DDL(P60)
### built-in types
char\ varchar\int\smallint\numeric\real, double precision \ float(P61)



# chapter4,5
## sql进阶部分
### view(P123)
从安全角度考虑，可能使用者不应该接触到数据库的全部，比如A不应该得到relation中salary这一attribute的值，所以可以用视图(不包含salary)，让使用者用这个视图
materialized views可以在relation改变时随着改变

### transactions(P129)
需要补充学习

### integrity constraints(P131)
constraints on a single relation:
not null, unqiue primary key, check clause
referential integiry:
有学到cascade、 set null\ set default等
comlex check conditions and assertions(这块没太懂)

### SQL Data types and schemas(P138)

