# pentaho_testing_suit

# jb_automate_testing

file_path is the path in which the jobs and resultant Excel will be produced.
main_job is the parent job for processing.

1. tr_get_metadata=> Populates Pictorial representation of jobs/transformation.
2. tr_validate_frameworks=> Serach for keywords ${common_frameworks},${common_frameworks1},${common_frameworks2} and verifies frameworks.
3.tr_validate_jos=> checks for hard coded parameters and checks if abort step is present or not.
4.tr_validate_db_conn_trans=> Validates DB connections and shows step descriptions.
5. tr_validate_api=> Validates if there are any API calls like GET/POST.
6. tr_validate_ssh_trans=> Validates if there are any Remote connection steps


#####Job Parmeter file from all environments########
This job is useful to gather job related parameters from various environments. For Demo it uses Dummy Oracle connections and assumes you have stored job related
parameters in database.

Input:
job_name=> parameter which is coma seperated with job names.

Output:
job_parameters.xls