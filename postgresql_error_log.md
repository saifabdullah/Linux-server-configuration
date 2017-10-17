2017-10-16 06:25:02.063 UTC [25883] catalog@catalog LOG:  could not receive data                                                       from client: Connection reset by peer
2017-10-16 07:54:14.820 UTC [13351] LOG:  received SIGHUP, reloading configurati                                                      on files
2017-10-16 08:00:41.868 UTC [32614] ubuntu@catalog ERROR:  syntax error at or ne                                                      ar "user" at character 13
2017-10-16 08:00:41.868 UTC [32614] ubuntu@catalog STATEMENT:  ALTER TABLE user                                                       ADD COLUMN id integer;
2017-10-16 08:02:14.491 UTC [32614] ubuntu@catalog ERROR:  syntax error at or ne                                                      ar "NOT" at character 41
2017-10-16 08:02:14.491 UTC [32614] ubuntu@catalog STATEMENT:  ALTER TABLE publi                                                      c.user ALTER COLUMN id NOT NULL;
2017-10-16 08:02:43.606 UTC [32614] ubuntu@catalog ERROR:  syntax error at or ne                                                      ar "PRIMARY_KEY" at character 45
2017-10-16 08:02:43.606 UTC [32614] ubuntu@catalog STATEMENT:  ALTER TABLE publi                                                      c.user ALTER COLUMN id SET PRIMARY_KEY;
2017-10-16 08:02:56.758 UTC [32614] ubuntu@catalog ERROR:  syntax error at or ne                                                      ar "PRIMARYKEY" at character 45
2017-10-16 08:02:56.758 UTC [32614] ubuntu@catalog STATEMENT:  ALTER TABLE publi                                                      c.user ALTER COLUMN id SET PRIMARYKEY;
2017-10-16 08:03:08.887 UTC [32614] ubuntu@catalog ERROR:  syntax error at or ne                                                      ar "UNIQUE" at character 45
2017-10-16 08:03:08.887 UTC [32614] ubuntu@catalog STATEMENT:  ALTER TABLE publi                                                      c.user ALTER COLUMN id SET UNIQUE;
2017-10-16 08:06:05.506 UTC [32614] ubuntu@catalog ERROR:  index "user_id" does                                                       not exist at character 29
2017-10-16 08:06:05.506 UTC [32614] ubuntu@catalog STATEMENT:  ALTER TABLE publi                                                      c.user ADD CONSTRAINT unique_id UNIQUE USING INDEX user_id;
2017-10-16 08:06:16.078 UTC [32614] ubuntu@catalog ERROR:  index "user_id" does                                                       not exist at character 29
2017-10-16 08:06:16.078 UTC [32614] ubuntu@catalog STATEMENT:  ALTER TABLE publi                                                      c.user ADD CONSTRAINT unique_id UNIQUE USING INDEX user_id;
2017-10-16 08:06:56.165 UTC [32614] ubuntu@catalog ERROR:  syntax error at or ne                                                      ar "user" at character 13
2017-10-16 08:06:56.165 UTC [32614] ubuntu@catalog STATEMENT:  ALTER TABLE user                                                       ADD CONSTRAINT unique_id UNIQUE USING INDEX user_id;
2017-10-16 08:07:08.979 UTC [32614] ubuntu@catalog ERROR:  index "user_id" does                                                       not exist at character 29
2017-10-16 08:07:08.979 UTC [32614] ubuntu@catalog STATEMENT:  ALTER TABLE publi                                                      c.user ADD CONSTRAINT unique_id UNIQUE USING INDEX user_id;
2017-10-16 08:07:41.262 UTC [32390] catalog@catalog ERROR:  null value in column                                                       "id" violates not-null constraint
2017-10-16 08:07:41.262 UTC [32390] catalog@catalog DETAIL:  Failing row contain                                                      s (saif, dhrubo.magazine@gmail.com, https://lh5.googleusercontent.com/-hcwca1lj0                                                      UU/AAAAAAAAAAI/AAAAA..., null).
2017-10-16 08:07:41.262 UTC [32390] catalog@catalog STATEMENT:  INSERT INTO "use                                                      r" (name, email, picture) VALUES ('saif', 'dhrubo.magazine@gmail.com', 'https://                                                      lh5.googleusercontent.com/-hcwca1lj0UU/AAAAAAAAAAI/AAAAAAAAADE/Paq6fakOfOk/photo                                                      .jpg') RETURNING "user".id
2017-10-16 11:35:36.634 UTC [1351] ubuntu@catalog ERROR:  syntax error at or nea                                                      r "COLUMN" at character 46
2017-10-16 11:35:36.634 UTC [1351] ubuntu@catalog STATEMENT:  ALTER TABLE public                                                      .user ALTER COLUMN id DROP COLUMN id;
2017-10-16 11:37:24.654 UTC [13351] LOG:  received SIGHUP, reloading configurati                                                      on files
2017-10-16 11:39:27.808 UTC [1412] ubuntu@catalog ERROR:  syntax error at or nea                                                      r "Session" at character 1
2017-10-16 11:39:27.808 UTC [1412] ubuntu@catalog STATEMENT:  Session rollback;
2017-10-16 11:39:42.752 UTC [1412] ubuntu@catalog ERROR:  syntax error at or nea                                                      r "session" at character 1
2017-10-16 11:39:42.752 UTC [1412] ubuntu@catalog STATEMENT:  session.rollback()                                                      ;
2017-10-16 11:40:30.683 UTC [1412] ubuntu@catalog WARNING:  there is no transact                                                      ion in progress
2017-10-16 11:41:07.282 UTC [1412] ubuntu@catalog ERROR:  syntax error at or nea                                                      r "session" at character 1
2017-10-16 11:41:07.282 UTC [1412] ubuntu@catalog STATEMENT:  session.commit()
        rollback
        rollback;
2017-10-17 06:25:01.684 UTC [32390] catalog@catalog LOG:  could not receive data                                                       from client: Connection reset by peer
2017-10-17 09:21:20.799 UTC [8843] ubuntu@catalog ERROR:  syntax error at or nea                                                      r "user" at character 12
2017-10-17 09:21:20.799 UTC [8843] ubuntu@catalog STATEMENT:  DROP table user
        DROP TABLE public.user;
2017-10-17 09:21:41.973 UTC [8843] ubuntu@catalog ERROR:  syntax error at or nea                                                      r "user" at character 12
2017-10-17 09:21:41.973 UTC [8843] ubuntu@catalog STATEMENT:  DROP TABLE user;
2017-10-17 09:23:48.002 UTC [8864] root@catalog ERROR:  syntax error at or near                                                       "user" at character 12
2017-10-17 09:23:48.002 UTC [8864] root@catalog STATEMENT:  drop table user
        DROP TABLE public.user;
2017-10-17 09:24:03.642 UTC [8864] root@catalog ERROR:  syntax error at or near                                                       "user" at character 12
2017-10-17 09:24:03.642 UTC [8864] root@catalog STATEMENT:  DROP TABLE user;
2017-10-17 09:52:19.778 UTC [9107] catalog@catalog LOG:  could not receive data                                                       from client: Connection reset by peer
ubuntu@ip-172-26-15-253:/var/log/postgresql$ 2017-10-16 11:39:27.808 UTC [1412] ubuntu@catalog ERROR:  syntax error at or nea                                                      r "Session" at character 1
2017-10-16: command not found
ubuntu@ip-172-26-15-253:/var/log/postgresql$ 2017-10-16 11:39:27.808 UTC [1412] ubuntu@catalog STATEMENT:  Session rollback;
2017-10-16: command not found
ubuntu@ip-172-26-15-253:/var/log/postgresql$ 2017-10-16 11:39:42.752 UTC [1412] ubuntu@catalog ERROR:  syntax error at or nea                                                      r "session" at character 1
2017-10-16: command not found
ubuntu@ip-172-26-15-253:/var/log/postgresql$ 2017-10-16 11:39:42.752 UTC [1412] ubuntu@catalog STATEMENT:  session.rollback()                                                      ;
-bash: syntax error near unexpected token `('
ubuntu@ip-172-26-15-253:/var/log/postgresql$ 2017-10-16 11:40:30.683 UTC [1412] ubuntu@catalog WARNING:  there is no transact                                                      ion in progress
2017-10-17 09:24:03.642 UTC [8864] root@catalog STATEMENT:  DROP TABLE user;
2017-10-17 09:52:19.778 UTC [9107] catalog@catalog LOG:  could not receive data                                                       from client: Connection reset by peer
2017-10-16: command not found
ubuntu@ip-172-26-15-253:/var/log/postgresql$ 2017-10-16 11:41:07.282 UTC [1412] ubuntu@catalog ERROR:  syntax error at or nea                                                      r "session" at character 1
2017-10-16: command not found
ubuntu@ip-172-26-15-253:/var/log/postgresql$ 2017-10-16 11:41:07.282 UTC [1412] ubuntu@catalog STATEMENT:  session.commit()
-bash: syntax error near unexpected token `('
ubuntu@ip-172-26-15-253:/var/log/postgresql$         rollback
rollback: command not found
ubuntu@ip-172-26-15-253:/var/log/postgresql$         rollback;
rollback: command not found
ubuntu@ip-172-26-15-253:/var/log/postgresql$ 2017-10-17 06:25:01.684 UTC [32390] catalog@catalog LOG:  could not receive data                                                       from client: Connection reset by peer
2017-10-17: command not found
ubuntu@ip-172-26-15-253:/var/log/postgresql$ 2017-10-17 09:21:20.799 UTC [8843] ubuntu@catalog ERROR:  syntax error at or nea                                                      r "user" at character 12
2017-10-17: command not found
ubuntu@ip-172-26-15-253:/var/log/postgresql$ 2017-10-17 09:21:20.799 UTC [8843] ubuntu@catalog STATEMENT:  DROP table user
2017-10-17: command not found
ubuntu@ip-172-26-15-253:/var/log/postgresql$         DROP TABLE public.user;
DROP: command not found
ubuntu@ip-172-26-15-253:/var/log/postgresql$ 2017-10-17 09:21:41.973 UTC [8843] ubuntu@catalog ERROR:  syntax error at or nea                                                      r "user" at character 12
2017-10-17: command not found
ubuntu@ip-172-26-15-253:/var/log/postgresql$ 2017-10-17 09:21:41.973 UTC [8843] ubuntu@catalog STATEMENT:  DROP TABLE user;
2017-10-17: command not found
ubuntu@ip-172-26-15-253:/var/log/postgresql$ 2017-10-17 09:23:48.002 UTC [8864] root@catalog ERROR:  syntax error at or near                                                       "user" at character 12
2017-10-17: command not found
ubuntu@ip-172-26-15-253:/var/log/postgresql$ 2017-10-17 09:23:48.002 UTC [8864] root@catalog STATEMENT:  drop table user
2017-10-17: command not found
ubuntu@ip-172-26-15-253:/var/log/postgresql$         DROP TABLE public.user;
DROP: command not found
ubuntu@ip-172-26-15-253:/var/log/postgresql$ 2017-10-17 09:24:03.642 UTC [8864] root@catalog ERROR:  syntax error at or near                                                       "user" at character 12
2017-10-17: command not found
ubuntu@ip-172-26-15-253:/var/log/postgresql$ 2017-10-17 09:24:03.642 UTC [8864] root@catalog STATEMENT:  DROP TABLE user;
2017-10-17: command not found
ubuntu@ip-172-26-15-253:/var/log/postgresql$ 2017-10-17 09:52:19.778 UTC [9107] catalog@catalog LOG:  could not receive data                                                       from client: Connection reset by peer
