# MySQL VIEWS

1. View is a virtual table created by a query by joining one or more tables. It is operated similarly to the base table but does not contain any data of its own.

3. The View and table have one main difference that the views are definitions built on top of other tables (or views). If any changes occur in the underlying table, the same changes are reflected in the View also.

4. **CREATE VIEW view_name AS SELECT columns FROM tables [WHERE conditions];**
5. **ALTER VIEW view_name AS SELECT columns FROM table WHERE conditions;**'
6. **DROP VIEW IF EXISTS view_name;**

7. **Example:**
   ```sql
   CREATE VIEW Trainer AS SELECT c.course_name, c.trainer, t.email FROM courses c, contact t WHERE c.id = t.id;
   ```