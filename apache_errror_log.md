[Tue Oct 17 06:25:01.714128 2017] [wsgi:warn] [pid 1365:tid 140249229596544] mod_wsgi: Compiled for Python/2.7.11.
[Tue Oct 17 06:25:01.714142 2017] [wsgi:warn] [pid 1365:tid 140249229596544] mod_wsgi: Runtime using Python/2.7.12.
[Tue Oct 17 06:25:01.714418 2017] [mpm_event:notice] [pid 1365:tid 140249229596544] AH00489: Apache/2.4.18 (Ubuntu) mod_wsgi/4.3.0 Python/2.7.12 configured -- resuming normal operations
[Tue Oct 17 06:25:01.714429 2017] [core:notice] [pid 1365:tid 140249229596544] AH00094: Command line: '/usr/sbin/apache2'
[Tue Oct 17 09:53:43.538359 2017] [wsgi:error] [pid 7593:tid 140249087604480] [remote 202.65.175.37:26449] [2017-10-17 09:53:43,536] ERROR in app: Exception on /gconnect [POST]
[Tue Oct 17 09:53:43.538387 2017] [wsgi:error] [pid 7593:tid 140249087604480] [remote 202.65.175.37:26449] Traceback (most recent call last):
[Tue Oct 17 09:53:43.538390 2017] [wsgi:error] [pid 7593:tid 140249087604480] [remote 202.65.175.37:26449]   File "/usr/local/lib/python2.7/dist-packages/flask/app.py", line 1982, in wsgi_app
[Tue Oct 17 09:53:43.538392 2017] [wsgi:error] [pid 7593:tid 140249087604480] [remote 202.65.175.37:26449]     response = self.full_dispatch_request()
[Tue Oct 17 09:53:43.538395 2017] [wsgi:error] [pid 7593:tid 140249087604480] [remote 202.65.175.37:26449]   File "/usr/local/lib/python2.7/dist-packages/flask/app.py", line 1614, in full_dispatch_request
[Tue Oct 17 09:53:43.538397 2017] [wsgi:error] [pid 7593:tid 140249087604480] [remote 202.65.175.37:26449]     rv = self.handle_user_exception(e)
[Tue Oct 17 09:53:43.538399 2017] [wsgi:error] [pid 7593:tid 140249087604480] [remote 202.65.175.37:26449]   File "/usr/local/lib/python2.7/dist-packages/flask/app.py", line 1517, in handle_user_exception
[Tue Oct 17 09:53:43.538401 2017] [wsgi:error] [pid 7593:tid 140249087604480] [remote 202.65.175.37:26449]     reraise(exc_type, exc_value, tb)
[Tue Oct 17 09:53:43.538403 2017] [wsgi:error] [pid 7593:tid 140249087604480] [remote 202.65.175.37:26449]   File "/usr/local/lib/python2.7/dist-packages/flask/app.py", line 1612, in full_dispatch_request
[Tue Oct 17 09:53:43.538405 2017] [wsgi:error] [pid 7593:tid 140249087604480] [remote 202.65.175.37:26449]     rv = self.dispatch_request()
[Tue Oct 17 09:53:43.538407 2017] [wsgi:error] [pid 7593:tid 140249087604480] [remote 202.65.175.37:26449]   File "/usr/local/lib/python2.7/dist-packages/flask/app.py", line 1598, in dispatch_request
[Tue Oct 17 09:53:43.538409 2017] [wsgi:error] [pid 7593:tid 140249087604480] [remote 202.65.175.37:26449]     return self.view_functions[rule.endpoint](**req.view_args)
[Tue Oct 17 09:53:43.538411 2017] [wsgi:error] [pid 7593:tid 140249087604480] [remote 202.65.175.37:26449]   File "/var/www/bcl2/bcl2.py", line 118, in gconnect
[Tue Oct 17 09:53:43.538413 2017] [wsgi:error] [pid 7593:tid 140249087604480] [remote 202.65.175.37:26449]     user_id = createUser(login_session)
[Tue Oct 17 09:53:43.538415 2017] [wsgi:error] [pid 7593:tid 140249087604480] [remote 202.65.175.37:26449]   File "/var/www/bcl2/bcl2.py", line 137, in createUser
[Tue Oct 17 09:53:43.538417 2017] [wsgi:error] [pid 7593:tid 140249087604480] [remote 202.65.175.37:26449]     ['email'],picture=login_session['picture'],id=login_session['user_id'])
[Tue Oct 17 09:53:43.538419 2017] [wsgi:error] [pid 7593:tid 140249087604480] [remote 202.65.175.37:26449]   File "/usr/local/lib/python2.7/dist-packages/werkzeug/local.py", line 377, in <lambda>
[Tue Oct 17 09:53:43.538421 2017] [wsgi:error] [pid 7593:tid 140249087604480] [remote 202.65.175.37:26449]     __getitem__ = lambda x, i: x._get_current_object()[i]
[Tue Oct 17 09:53:43.538423 2017] [wsgi:error] [pid 7593:tid 140249087604480] [remote 202.65.175.37:26449] KeyError: 'user_id'
[Tue Oct 17 09:54:34.975116 2017] [wsgi:error] [pid 7593:tid 140249087604480] [remote 202.65.175.37:26193] [2017-10-17 09:54:34,974] ERROR in app: Exception on /gconnect [POST]
[Tue Oct 17 09:54:34.975144 2017] [wsgi:error] [pid 7593:tid 140249087604480] [remote 202.65.175.37:26193] Traceback (most recent call last):
[Tue Oct 17 09:54:34.975147 2017] [wsgi:error] [pid 7593:tid 140249087604480] [remote 202.65.175.37:26193]   File "/usr/local/lib/python2.7/dist-packages/flask/app.py", line 1982, in wsgi_app
[Tue Oct 17 09:54:34.975157 2017] [wsgi:error] [pid 7593:tid 140249087604480] [remote 202.65.175.37:26193]     response = self.full_dispatch_request()
[Tue Oct 17 09:54:34.975159 2017] [wsgi:error] [pid 7593:tid 140249087604480] [remote 202.65.175.37:26193]   File "/usr/local/lib/python2.7/dist-packages/flask/app.py", line 1614, in full_dispatch_request
[Tue Oct 17 09:54:34.975161 2017] [wsgi:error] [pid 7593:tid 140249087604480] [remote 202.65.175.37:26193]     rv = self.handle_user_exception(e)
[Tue Oct 17 09:54:34.975163 2017] [wsgi:error] [pid 7593:tid 140249087604480] [remote 202.65.175.37:26193]   File "/usr/local/lib/python2.7/dist-packages/flask/app.py", line 1517, in handle_user_exception
[Tue Oct 17 09:54:34.975165 2017] [wsgi:error] [pid 7593:tid 140249087604480] [remote 202.65.175.37:26193]     reraise(exc_type, exc_value, tb)
[Tue Oct 17 09:54:34.975167 2017] [wsgi:error] [pid 7593:tid 140249087604480] [remote 202.65.175.37:26193]   File "/usr/local/lib/python2.7/dist-packages/flask/app.py", line 1612, in full_dispatch_request
[Tue Oct 17 09:54:34.975169 2017] [wsgi:error] [pid 7593:tid 140249087604480] [remote 202.65.175.37:26193]     rv = self.dispatch_request()
[Tue Oct 17 09:54:34.975170 2017] [wsgi:error] [pid 7593:tid 140249087604480] [remote 202.65.175.37:26193]   File "/usr/local/lib/python2.7/dist-packages/flask/app.py", line 1598, in dispatch_request
[Tue Oct 17 09:54:34.975172 2017] [wsgi:error] [pid 7593:tid 140249087604480] [remote 202.65.175.37:26193]     return self.view_functions[rule.endpoint](**req.view_args)
[Tue Oct 17 09:54:34.975174 2017] [wsgi:error] [pid 7593:tid 140249087604480] [remote 202.65.175.37:26193]   File "/var/www/bcl2/bcl2.py", line 118, in gconnect
[Tue Oct 17 09:54:34.975176 2017] [wsgi:error] [pid 7593:tid 140249087604480] [remote 202.65.175.37:26193]     user_id = createUser(login_session)
[Tue Oct 17 09:54:34.975177 2017] [wsgi:error] [pid 7593:tid 140249087604480] [remote 202.65.175.37:26193]   File "/var/www/bcl2/bcl2.py", line 137, in createUser
[Tue Oct 17 09:54:34.975179 2017] [wsgi:error] [pid 7593:tid 140249087604480] [remote 202.65.175.37:26193]     ['email'],picture=login_session['picture'],id=login_session['user_id'])
[Tue Oct 17 09:54:34.975181 2017] [wsgi:error] [pid 7593:tid 140249087604480] [remote 202.65.175.37:26193]   File "/usr/local/lib/python2.7/dist-packages/werkzeug/local.py", line 377, in <lambda>
[Tue Oct 17 09:54:34.975183 2017] [wsgi:error] [pid 7593:tid 140249087604480] [remote 202.65.175.37:26193]     __getitem__ = lambda x, i: x._get_current_object()[i]
[Tue Oct 17 09:54:34.975185 2017] [wsgi:error] [pid 7593:tid 140249087604480] [remote 202.65.175.37:26193] KeyError: 'user_id'
[Tue Oct 17 09:59:20.330084 2017] [wsgi:error] [pid 7593:tid 140249121208064] [remote 202.65.175.37:35656] [2017-10-17 09:59:20,329] ERROR in app: Exception on /gconnect [POST]
[Tue Oct 17 09:59:20.330110 2017] [wsgi:error] [pid 7593:tid 140249121208064] [remote 202.65.175.37:35656] Traceback (most recent call last):
[Tue Oct 17 09:59:20.330113 2017] [wsgi:error] [pid 7593:tid 140249121208064] [remote 202.65.175.37:35656]   File "/usr/local/lib/python2.7/dist-packages/flask/app.py", line 1982, in wsgi_app
[Tue Oct 17 09:59:20.330115 2017] [wsgi:error] [pid 7593:tid 140249121208064] [remote 202.65.175.37:35656]     response = self.full_dispatch_request()
[Tue Oct 17 09:59:20.330118 2017] [wsgi:error] [pid 7593:tid 140249121208064] [remote 202.65.175.37:35656]   File "/usr/local/lib/python2.7/dist-packages/flask/app.py", line 1614, in full_dispatch_request
[Tue Oct 17 09:59:20.330120 2017] [wsgi:error] [pid 7593:tid 140249121208064] [remote 202.65.175.37:35656]     rv = self.handle_user_exception(e)
[Tue Oct 17 09:59:20.330122 2017] [wsgi:error] [pid 7593:tid 140249121208064] [remote 202.65.175.37:35656]   File "/usr/local/lib/python2.7/dist-packages/flask/app.py", line 1517, in handle_user_exception
[Tue Oct 17 09:59:20.330144 2017] [wsgi:error] [pid 7593:tid 140249121208064] [remote 202.65.175.37:35656]     reraise(exc_type, exc_value, tb)
[Tue Oct 17 09:59:20.330146 2017] [wsgi:error] [pid 7593:tid 140249121208064] [remote 202.65.175.37:35656]   File "/usr/local/lib/python2.7/dist-packages/flask/app.py", line 1612, in full_dispatch_request
[Tue Oct 17 09:59:20.330147 2017] [wsgi:error] [pid 7593:tid 140249121208064] [remote 202.65.175.37:35656]     rv = self.dispatch_request()
[Tue Oct 17 09:59:20.330149 2017] [wsgi:error] [pid 7593:tid 140249121208064] [remote 202.65.175.37:35656]   File "/usr/local/lib/python2.7/dist-packages/flask/app.py", line 1598, in dispatch_request
[Tue Oct 17 09:59:20.330151 2017] [wsgi:error] [pid 7593:tid 140249121208064] [remote 202.65.175.37:35656]     return self.view_functions[rule.endpoint](**req.view_args)
[Tue Oct 17 09:59:20.330153 2017] [wsgi:error] [pid 7593:tid 140249121208064] [remote 202.65.175.37:35656]   File "/var/www/bcl2/bcl2.py", line 118, in gconnect
[Tue Oct 17 09:59:20.330154 2017] [wsgi:error] [pid 7593:tid 140249121208064] [remote 202.65.175.37:35656]     user_id = createUser(login_session)
[Tue Oct 17 09:59:20.330156 2017] [wsgi:error] [pid 7593:tid 140249121208064] [remote 202.65.175.37:35656]   File "/var/www/bcl2/bcl2.py", line 137, in createUser
[Tue Oct 17 09:59:20.330158 2017] [wsgi:error] [pid 7593:tid 140249121208064] [remote 202.65.175.37:35656]     ['email'],picture=login_session['picture'])
[Tue Oct 17 09:59:20.330159 2017] [wsgi:error] [pid 7593:tid 140249121208064] [remote 202.65.175.37:35656]   File "/usr/local/lib/python2.7/dist-packages/werkzeug/local.py", line 377, in <lambda>
[Tue Oct 17 09:59:20.330161 2017] [wsgi:error] [pid 7593:tid 140249121208064] [remote 202.65.175.37:35656]     __getitem__ = lambda x, i: x._get_current_object()[i]
[Tue Oct 17 09:59:20.330163 2017] [wsgi:error] [pid 7593:tid 140249121208064] [remote 202.65.175.37:35656] KeyError: 'user_id'
[Tue Oct 17 09:59:27.255525 2017] [wsgi:error] [pid 7593:tid 140249087604480] [remote 202.65.175.37:26193] [2017-10-17 09:59:27,255] ERROR in app: Exception on /gconnect [POST]
[Tue Oct 17 09:59:27.255550 2017] [wsgi:error] [pid 7593:tid 140249087604480] [remote 202.65.175.37:26193] Traceback (most recent call last):
[Tue Oct 17 09:59:27.255552 2017] [wsgi:error] [pid 7593:tid 140249087604480] [remote 202.65.175.37:26193]   File "/usr/local/lib/python2.7/dist-packages/flask/app.py", line 1982, in wsgi_app
[Tue Oct 17 09:59:27.255555 2017] [wsgi:error] [pid 7593:tid 140249087604480] [remote 202.65.175.37:26193]     response = self.full_dispatch_request()
[Tue Oct 17 09:59:27.255557 2017] [wsgi:error] [pid 7593:tid 140249087604480] [remote 202.65.175.37:26193]   File "/usr/local/lib/python2.7/dist-packages/flask/app.py", line 1614, in full_dispatch_request
[Tue Oct 17 09:59:27.255559 2017] [wsgi:error] [pid 7593:tid 140249087604480] [remote 202.65.175.37:26193]     rv = self.handle_user_exception(e)
[Tue Oct 17 09:59:27.255561 2017] [wsgi:error] [pid 7593:tid 140249087604480] [remote 202.65.175.37:26193]   File "/usr/local/lib/python2.7/dist-packages/flask/app.py", line 1517, in handle_user_exception
[Tue Oct 17 09:59:27.255562 2017] [wsgi:error] [pid 7593:tid 140249087604480] [remote 202.65.175.37:26193]     reraise(exc_type, exc_value, tb)
[Tue Oct 17 09:59:27.255564 2017] [wsgi:error] [pid 7593:tid 140249087604480] [remote 202.65.175.37:26193]   File "/usr/local/lib/python2.7/dist-packages/flask/app.py", line 1612, in full_dispatch_request
[Tue Oct 17 09:59:27.255566 2017] [wsgi:error] [pid 7593:tid 140249087604480] [remote 202.65.175.37:26193]     rv = self.dispatch_request()
[Tue Oct 17 09:59:27.255568 2017] [wsgi:error] [pid 7593:tid 140249087604480] [remote 202.65.175.37:26193]   File "/usr/local/lib/python2.7/dist-packages/flask/app.py", line 1598, in dispatch_request
[Tue Oct 17 09:59:27.255570 2017] [wsgi:error] [pid 7593:tid 140249087604480] [remote 202.65.175.37:26193]     return self.view_functions[rule.endpoint](**req.view_args)
[Tue Oct 17 09:59:27.255572 2017] [wsgi:error] [pid 7593:tid 140249087604480] [remote 202.65.175.37:26193]   File "/var/www/bcl2/bcl2.py", line 118, in gconnect
[Tue Oct 17 09:59:27.255584 2017] [wsgi:error] [pid 7593:tid 140249087604480] [remote 202.65.175.37:26193]     user_id = createUser(login_session)
[Tue Oct 17 09:59:27.255586 2017] [wsgi:error] [pid 7593:tid 140249087604480] [remote 202.65.175.37:26193]   File "/var/www/bcl2/bcl2.py", line 137, in createUser
[Tue Oct 17 09:59:27.255588 2017] [wsgi:error] [pid 7593:tid 140249087604480] [remote 202.65.175.37:26193]     ['email'],picture=login_session['picture'])
[Tue Oct 17 09:59:27.255589 2017] [wsgi:error] [pid 7593:tid 140249087604480] [remote 202.65.175.37:26193]   File "/usr/local/lib/python2.7/dist-packages/werkzeug/local.py", line 377, in <lambda>
[Tue Oct 17 09:59:27.255591 2017] [wsgi:error] [pid 7593:tid 140249087604480] [remote 202.65.175.37:26193]     __getitem__ = lambda x, i: x._get_current_object()[i]
[Tue Oct 17 09:59:27.255593 2017] [wsgi:error] [pid 7593:tid 140249087604480] [remote 202.65.175.37:26193] KeyError: 'user_id'
[Tue Oct 17 10:01:50.199521 2017] [wsgi:error] [pid 7593:tid 140249121208064] [remote 202.65.175.37:34632] [2017-10-17 10:01:50,199] ERROR in app: Exception on /gconnect [POST]
[Tue Oct 17 10:01:50.199548 2017] [wsgi:error] [pid 7593:tid 140249121208064] [remote 202.65.175.37:34632] Traceback (most recent call last):
[Tue Oct 17 10:01:50.199551 2017] [wsgi:error] [pid 7593:tid 140249121208064] [remote 202.65.175.37:34632]   File "/usr/local/lib/python2.7/dist-packages/flask/app.py", line 1982, in wsgi_app
[Tue Oct 17 10:01:50.199553 2017] [wsgi:error] [pid 7593:tid 140249121208064] [remote 202.65.175.37:34632]     response = self.full_dispatch_request()
[Tue Oct 17 10:01:50.199556 2017] [wsgi:error] [pid 7593:tid 140249121208064] [remote 202.65.175.37:34632]   File "/usr/local/lib/python2.7/dist-packages/flask/app.py", line 1614, in full_dispatch_request
[Tue Oct 17 10:01:50.199558 2017] [wsgi:error] [pid 7593:tid 140249121208064] [remote 202.65.175.37:34632]     rv = self.handle_user_exception(e)
[Tue Oct 17 10:01:50.199560 2017] [wsgi:error] [pid 7593:tid 140249121208064] [remote 202.65.175.37:34632]   File "/usr/local/lib/python2.7/dist-packages/flask/app.py", line 1517, in handle_user_exception
[Tue Oct 17 10:01:50.199562 2017] [wsgi:error] [pid 7593:tid 140249121208064] [remote 202.65.175.37:34632]     reraise(exc_type, exc_value, tb)
[Tue Oct 17 10:01:50.199564 2017] [wsgi:error] [pid 7593:tid 140249121208064] [remote 202.65.175.37:34632]   File "/usr/local/lib/python2.7/dist-packages/flask/app.py", line 1612, in full_dispatch_request
[Tue Oct 17 10:01:50.199566 2017] [wsgi:error] [pid 7593:tid 140249121208064] [remote 202.65.175.37:34632]     rv = self.dispatch_request()
[Tue Oct 17 10:01:50.199568 2017] [wsgi:error] [pid 7593:tid 140249121208064] [remote 202.65.175.37:34632]   File "/usr/local/lib/python2.7/dist-packages/flask/app.py", line 1598, in dispatch_request
[Tue Oct 17 10:01:50.199570 2017] [wsgi:error] [pid 7593:tid 140249121208064] [remote 202.65.175.37:34632]     return self.view_functions[rule.endpoint](**req.view_args)
[Tue Oct 17 10:01:50.199572 2017] [wsgi:error] [pid 7593:tid 140249121208064] [remote 202.65.175.37:34632]   File "/var/www/bcl2/bcl2.py", line 118, in gconnect
[Tue Oct 17 10:01:50.199574 2017] [wsgi:error] [pid 7593:tid 140249121208064] [remote 202.65.175.37:34632]     user_id = createUser(login_session)
[Tue Oct 17 10:01:50.199576 2017] [wsgi:error] [pid 7593:tid 140249121208064] [remote 202.65.175.37:34632]   File "/var/www/bcl2/bcl2.py", line 137, in createUser
[Tue Oct 17 10:01:50.199581 2017] [wsgi:error] [pid 7593:tid 140249121208064] [remote 202.65.175.37:34632]     ['email'],picture=login_session['picture'])
[Tue Oct 17 10:01:50.199583 2017] [wsgi:error] [pid 7593:tid 140249121208064] [remote 202.65.175.37:34632]   File "/usr/local/lib/python2.7/dist-packages/werkzeug/local.py", line 377, in <lambda>
[Tue Oct 17 10:01:50.199585 2017] [wsgi:error] [pid 7593:tid 140249121208064] [remote 202.65.175.37:34632]     __getitem__ = lambda x, i: x._get_current_object()[i]
[Tue Oct 17 10:01:50.199602 2017] [wsgi:error] [pid 7593:tid 140249121208064] [remote 202.65.175.37:34632] KeyError: 'user_id'
[Tue Oct 17 10:12:57.259393 2017] [wsgi:error] [pid 7593:tid 140249087604480] [remote 202.65.175.37:35656] [2017-10-17 10:12:57,259] ERROR in app: Exception on /gconnect [POST]
[Tue Oct 17 10:12:57.259416 2017] [wsgi:error] [pid 7593:tid 140249087604480] [remote 202.65.175.37:35656] Traceback (most recent call last):
[Tue Oct 17 10:12:57.259419 2017] [wsgi:error] [pid 7593:tid 140249087604480] [remote 202.65.175.37:35656]   File "/usr/local/lib/python2.7/dist-packages/flask/app.py", line 1982, in wsgi_app
[Tue Oct 17 10:12:57.259422 2017] [wsgi:error] [pid 7593:tid 140249087604480] [remote 202.65.175.37:35656]     response = self.full_dispatch_request()
[Tue Oct 17 10:12:57.259425 2017] [wsgi:error] [pid 7593:tid 140249087604480] [remote 202.65.175.37:35656]   File "/usr/local/lib/python2.7/dist-packages/flask/app.py", line 1614, in full_dispatch_request
[Tue Oct 17 10:12:57.259427 2017] [wsgi:error] [pid 7593:tid 140249087604480] [remote 202.65.175.37:35656]     rv = self.handle_user_exception(e)
[Tue Oct 17 10:12:57.259430 2017] [wsgi:error] [pid 7593:tid 140249087604480] [remote 202.65.175.37:35656]   File "/usr/local/lib/python2.7/dist-packages/flask/app.py", line 1517, in handle_user_exception
[Tue Oct 17 10:12:57.259432 2017] [wsgi:error] [pid 7593:tid 140249087604480] [remote 202.65.175.37:35656]     reraise(exc_type, exc_value, tb)
[Tue Oct 17 10:12:57.259434 2017] [wsgi:error] [pid 7593:tid 140249087604480] [remote 202.65.175.37:35656]   File "/usr/local/lib/python2.7/dist-packages/flask/app.py", line 1612, in full_dispatch_request
[Tue Oct 17 10:12:57.259436 2017] [wsgi:error] [pid 7593:tid 140249087604480] [remote 202.65.175.37:35656]     rv = self.dispatch_request()
[Tue Oct 17 10:12:57.259439 2017] [wsgi:error] [pid 7593:tid 140249087604480] [remote 202.65.175.37:35656]   File "/usr/local/lib/python2.7/dist-packages/flask/app.py", line 1598, in dispatch_request
[Tue Oct 17 10:12:57.259441 2017] [wsgi:error] [pid 7593:tid 140249087604480] [remote 202.65.175.37:35656]     return self.view_functions[rule.endpoint](**req.view_args)
[Tue Oct 17 10:12:57.259443 2017] [wsgi:error] [pid 7593:tid 140249087604480] [remote 202.65.175.37:35656]   File "/var/www/bcl2/bcl2.py", line 118, in gconnect
[Tue Oct 17 10:12:57.259445 2017] [wsgi:error] [pid 7593:tid 140249087604480] [remote 202.65.175.37:35656]     user_id = createUser(login_session)
[Tue Oct 17 10:12:57.259447 2017] [wsgi:error] [pid 7593:tid 140249087604480] [remote 202.65.175.37:35656]   File "/var/www/bcl2/bcl2.py", line 137, in createUser
[Tue Oct 17 10:12:57.259449 2017] [wsgi:error] [pid 7593:tid 140249087604480] [remote 202.65.175.37:35656]     ['email'],picture=login_session['picture'],id=login_session['user_id'])
[Tue Oct 17 10:12:57.259451 2017] [wsgi:error] [pid 7593:tid 140249087604480] [remote 202.65.175.37:35656]   File "/usr/local/lib/python2.7/dist-packages/werkzeug/local.py", line 377, in <lambda>
[Tue Oct 17 10:12:57.259453 2017] [wsgi:error] [pid 7593:tid 140249087604480] [remote 202.65.175.37:35656]     __getitem__ = lambda x, i: x._get_current_object()[i]
[Tue Oct 17 10:12:57.259455 2017] [wsgi:error] [pid 7593:tid 140249087604480] [remote 202.65.175.37:35656] KeyError: 'user_id'
[Tue Oct 17 10:18:43.842013 2017] [wsgi:error] [pid 7593:tid 140249087604480] [remote 202.65.175.37:35656] [2017-10-17 10:18:43,841] ERROR in app: Exception on /gconnect [POST]
[Tue Oct 17 10:18:43.842037 2017] [wsgi:error] [pid 7593:tid 140249087604480] [remote 202.65.175.37:35656] Traceback (most recent call last):
[Tue Oct 17 10:18:43.842040 2017] [wsgi:error] [pid 7593:tid 140249087604480] [remote 202.65.175.37:35656]   File "/usr/local/lib/python2.7/dist-packages/flask/app.py", line 1982, in wsgi_app
[Tue Oct 17 10:18:43.842042 2017] [wsgi:error] [pid 7593:tid 140249087604480] [remote 202.65.175.37:35656]     response = self.full_dispatch_request()
[Tue Oct 17 10:18:43.842044 2017] [wsgi:error] [pid 7593:tid 140249087604480] [remote 202.65.175.37:35656]   File "/usr/local/lib/python2.7/dist-packages/flask/app.py", line 1614, in full_dispatch_request
[Tue Oct 17 10:18:43.842054 2017] [wsgi:error] [pid 7593:tid 140249087604480] [remote 202.65.175.37:35656]     rv = self.handle_user_exception(e)
[Tue Oct 17 10:18:43.842056 2017] [wsgi:error] [pid 7593:tid 140249087604480] [remote 202.65.175.37:35656]   File "/usr/local/lib/python2.7/dist-packages/flask/app.py", line 1517, in handle_user_exception
[Tue Oct 17 10:18:43.842058 2017] [wsgi:error] [pid 7593:tid 140249087604480] [remote 202.65.175.37:35656]     reraise(exc_type, exc_value, tb)
[Tue Oct 17 10:18:43.842059 2017] [wsgi:error] [pid 7593:tid 140249087604480] [remote 202.65.175.37:35656]   File "/usr/local/lib/python2.7/dist-packages/flask/app.py", line 1612, in full_dispatch_request
[Tue Oct 17 10:18:43.842061 2017] [wsgi:error] [pid 7593:tid 140249087604480] [remote 202.65.175.37:35656]     rv = self.dispatch_request()
[Tue Oct 17 10:18:43.842063 2017] [wsgi:error] [pid 7593:tid 140249087604480] [remote 202.65.175.37:35656]   File "/usr/local/lib/python2.7/dist-packages/flask/app.py", line 1598, in dispatch_request
[Tue Oct 17 10:18:43.842065 2017] [wsgi:error] [pid 7593:tid 140249087604480] [remote 202.65.175.37:35656]     return self.view_functions[rule.endpoint](**req.view_args)
[Tue Oct 17 10:18:43.842066 2017] [wsgi:error] [pid 7593:tid 140249087604480] [remote 202.65.175.37:35656]   File "/var/www/bcl2/bcl2.py", line 118, in gconnect
[Tue Oct 17 10:18:43.842068 2017] [wsgi:error] [pid 7593:tid 140249087604480] [remote 202.65.175.37:35656]     user_id = createUser(login_session)
[Tue Oct 17 10:18:43.842070 2017] [wsgi:error] [pid 7593:tid 140249087604480] [remote 202.65.175.37:35656]   File "/var/www/bcl2/bcl2.py", line 137, in createUser
[Tue Oct 17 10:18:43.842071 2017] [wsgi:error] [pid 7593:tid 140249087604480] [remote 202.65.175.37:35656]     ['email'],picture=login_session['picture'])
[Tue Oct 17 10:18:43.842073 2017] [wsgi:error] [pid 7593:tid 140249087604480] [remote 202.65.175.37:35656]   File "/usr/local/lib/python2.7/dist-packages/werkzeug/local.py", line 377, in <lambda>
[Tue Oct 17 10:18:43.842075 2017] [wsgi:error] [pid 7593:tid 140249087604480] [remote 202.65.175.37:35656]     __getitem__ = lambda x, i: x._get_current_object()[i]
[Tue Oct 17 10:18:43.842076 2017] [wsgi:error] [pid 7593:tid 140249087604480] [remote 202.65.175.37:35656] KeyError: 'user_id'
[Tue Oct 17 10:47:50.134671 2017] [wsgi:error] [pid 7593:tid 140249121208064] [remote 202.65.175.37:26193] [2017-10-17 10:47:50,134] ERROR in app: Exception on /gconnect [POST]
[Tue Oct 17 10:47:50.134698 2017] [wsgi:error] [pid 7593:tid 140249121208064] [remote 202.65.175.37:26193] Traceback (most recent call last):
[Tue Oct 17 10:47:50.134706 2017] [wsgi:error] [pid 7593:tid 140249121208064] [remote 202.65.175.37:26193]   File "/usr/local/lib/python2.7/dist-packages/flask/app.py", line 1982, in wsgi_app
[Tue Oct 17 10:47:50.134709 2017] [wsgi:error] [pid 7593:tid 140249121208064] [remote 202.65.175.37:26193]     response = self.full_dispatch_request()
[Tue Oct 17 10:47:50.134711 2017] [wsgi:error] [pid 7593:tid 140249121208064] [remote 202.65.175.37:26193]   File "/usr/local/lib/python2.7/dist-packages/flask/app.py", line 1614, in full_dispatch_request
[Tue Oct 17 10:47:50.134713 2017] [wsgi:error] [pid 7593:tid 140249121208064] [remote 202.65.175.37:26193]     rv = self.handle_user_exception(e)
[Tue Oct 17 10:47:50.134715 2017] [wsgi:error] [pid 7593:tid 140249121208064] [remote 202.65.175.37:26193]   File "/usr/local/lib/python2.7/dist-packages/flask/app.py", line 1517, in handle_user_exception
[Tue Oct 17 10:47:50.134717 2017] [wsgi:error] [pid 7593:tid 140249121208064] [remote 202.65.175.37:26193]     reraise(exc_type, exc_value, tb)
[Tue Oct 17 10:47:50.134719 2017] [wsgi:error] [pid 7593:tid 140249121208064] [remote 202.65.175.37:26193]   File "/usr/local/lib/python2.7/dist-packages/flask/app.py", line 1612, in full_dispatch_request
[Tue Oct 17 10:47:50.134721 2017] [wsgi:error] [pid 7593:tid 140249121208064] [remote 202.65.175.37:26193]     rv = self.dispatch_request()
[Tue Oct 17 10:47:50.134733 2017] [wsgi:error] [pid 7593:tid 140249121208064] [remote 202.65.175.37:26193]   File "/usr/local/lib/python2.7/dist-packages/flask/app.py", line 1598, in dispatch_request
[Tue Oct 17 10:47:50.134735 2017] [wsgi:error] [pid 7593:tid 140249121208064] [remote 202.65.175.37:26193]     return self.view_functions[rule.endpoint](**req.view_args)
[Tue Oct 17 10:47:50.134737 2017] [wsgi:error] [pid 7593:tid 140249121208064] [remote 202.65.175.37:26193]   File "/var/www/bcl2/bcl2.py", line 51, in gconnect
[Tue Oct 17 10:47:50.134739 2017] [wsgi:error] [pid 7593:tid 140249121208064] [remote 202.65.175.37:26193]     if request.args.get('state') != login_session['state']:
[Tue Oct 17 10:47:50.134741 2017] [wsgi:error] [pid 7593:tid 140249121208064] [remote 202.65.175.37:26193]   File "/usr/local/lib/python2.7/dist-packages/werkzeug/local.py", line 377, in <lambda>
[Tue Oct 17 10:47:50.134742 2017] [wsgi:error] [pid 7593:tid 140249121208064] [remote 202.65.175.37:26193]     __getitem__ = lambda x, i: x._get_current_object()[i]
[Tue Oct 17 10:47:50.134744 2017] [wsgi:error] [pid 7593:tid 140249121208064] [remote 202.65.175.37:26193] KeyError: 'state'
[Tue Oct 17 10:58:27.525922 2017] [wsgi:error] [pid 7593:tid 140249121208064] [remote 202.65.175.37:34632] [2017-10-17 10:58:27,524] ERROR in app: Exception on /gconnect [POST]
[Tue Oct 17 10:58:27.525949 2017] [wsgi:error] [pid 7593:tid 140249121208064] [remote 202.65.175.37:34632] Traceback (most recent call last):
[Tue Oct 17 10:58:27.525953 2017] [wsgi:error] [pid 7593:tid 140249121208064] [remote 202.65.175.37:34632]   File "/usr/local/lib/python2.7/dist-packages/flask/app.py", line 1982, in wsgi_app
[Tue Oct 17 10:58:27.525955 2017] [wsgi:error] [pid 7593:tid 140249121208064] [remote 202.65.175.37:34632]     response = self.full_dispatch_request()
[Tue Oct 17 10:58:27.525958 2017] [wsgi:error] [pid 7593:tid 140249121208064] [remote 202.65.175.37:34632]   File "/usr/local/lib/python2.7/dist-packages/flask/app.py", line 1614, in full_dispatch_request
[Tue Oct 17 10:58:27.525960 2017] [wsgi:error] [pid 7593:tid 140249121208064] [remote 202.65.175.37:34632]     rv = self.handle_user_exception(e)
[Tue Oct 17 10:58:27.525962 2017] [wsgi:error] [pid 7593:tid 140249121208064] [remote 202.65.175.37:34632]   File "/usr/local/lib/python2.7/dist-packages/flask/app.py", line 1517, in handle_user_exception
[Tue Oct 17 10:58:27.525964 2017] [wsgi:error] [pid 7593:tid 140249121208064] [remote 202.65.175.37:34632]     reraise(exc_type, exc_value, tb)
[Tue Oct 17 10:58:27.525966 2017] [wsgi:error] [pid 7593:tid 140249121208064] [remote 202.65.175.37:34632]   File "/usr/local/lib/python2.7/dist-packages/flask/app.py", line 1612, in full_dispatch_request
[Tue Oct 17 10:58:27.525969 2017] [wsgi:error] [pid 7593:tid 140249121208064] [remote 202.65.175.37:34632]     rv = self.dispatch_request()
[Tue Oct 17 10:58:27.525971 2017] [wsgi:error] [pid 7593:tid 140249121208064] [remote 202.65.175.37:34632]   File "/usr/local/lib/python2.7/dist-packages/flask/app.py", line 1598, in dispatch_request
[Tue Oct 17 10:58:27.525973 2017] [wsgi:error] [pid 7593:tid 140249121208064] [remote 202.65.175.37:34632]     return self.view_functions[rule.endpoint](**req.view_args)
[Tue Oct 17 10:58:27.525975 2017] [wsgi:error] [pid 7593:tid 140249121208064] [remote 202.65.175.37:34632]   File "/var/www/bcl2/bcl2.py", line 118, in gconnect
[Tue Oct 17 10:58:27.525977 2017] [wsgi:error] [pid 7593:tid 140249121208064] [remote 202.65.175.37:34632]     user_id = createUser(login_session)
[Tue Oct 17 10:58:27.525979 2017] [wsgi:error] [pid 7593:tid 140249121208064] [remote 202.65.175.37:34632]   File "/var/www/bcl2/bcl2.py", line 137, in createUser
[Tue Oct 17 10:58:27.525981 2017] [wsgi:error] [pid 7593:tid 140249121208064] [remote 202.65.175.37:34632]     session.add(newUser)
[Tue Oct 17 10:58:27.525982 2017] [wsgi:error] [pid 7593:tid 140249121208064] [remote 202.65.175.37:34632]   File "/usr/local/lib/python2.7/dist-packages/werkzeug/local.py", line 377, in <lambda>
[Tue Oct 17 10:58:27.525991 2017] [wsgi:error] [pid 7593:tid 140249121208064] [remote 202.65.175.37:34632]     __getitem__ = lambda x, i: x._get_current_object()[i]
[Tue Oct 17 10:58:27.525993 2017] [wsgi:error] [pid 7593:tid 140249121208064] [remote 202.65.175.37:34632] KeyError: 'user_id'
