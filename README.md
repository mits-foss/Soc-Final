# Soc-Final
Putting all together, lets see
todo-
just use localstoage for user_id(the github_login id) . No need to use the tokens for auth headers. Tokens used only for cron job. 

point system:
If people come to offline session, give 5 points to user upon showing certificate( points will be given by admins)
have an admin route( with user and password) 

cron job
If PR status is open, only then add to table. 
If pr status is closed and not in table, skip
If pr exists in pr_table and pr_table_status=open,  and current status(from the cron job) = merged, 1 point, set pr_table_status=merged

OAUTH
change the logic. Convert backend to frontend
better if react does oauth instead of backend. 

Routes from frontend
Dashboard-User details(should the repos contributed in filters.txt,PRs opened and closed in these filters.txt) -> in backend, name should be get_user_info, currently dashboard