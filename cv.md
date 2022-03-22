# Victoria Tsymbal
### Senior Engineer

*********

### Contacts:
**Phone:** +79154606984 <br>
**E-mail:** [tstoti@ya.ru](mailto:tstoti@ya.ru)<br>
**Telegram:** @ts_tory<br>
**GitHub:** [tstori](https://github.com/tstori)<br>
**Habr Career:** [tsyimbalviktoriya](https://career.habr.com/tsyimbalviktoriya)

*********

### About Me

At the moment I work as a data quality engineer in a company providing mobile communication services in Russia.<br>
Basically my job is the elimination of problems associated with data distortion, as well as the writing of automatic control procedures for checking data quality.<br>
I would really like to gain knowledge and skills in the frontend, for further participation in projects for the development of internal web services of the company, including projects related to data quality (development of a dashboard, monitoring system, etc.)<br>

*********

### Skills:

- HTML5, CSS3
- JavaScript Basics
- PL/SQL at the level of writing stored procedures, Bash
- Git, GitHub
- VS Code, PL/SQL Developer

*********

### Code example:

Checking the readiness of all data. Сode snippet.

```SQL
    select count(1),
           sum(t.checks_sys1),
           sum(checks_mnp_sys2),
           sum(checks_mnp_sys3),
           sum(checks_mnp_sys1_new_req),
           sum(checks)
    into v_all_row,
         v_checks_sys1,
         v_checks_mnp_sys2,
         v_checks_mnp_sys3,
         v_checks_mnp_sys1_new_req,
         v_checks
    from PUBLIC_TEMP.sms_checks t
    where t.rep_id = in_rep_id;

    public.logs_p.write_detail_log('v_all_row = ' || v_all_row
                                    || chr(13) || chr(10) || 'v_checks_sys1 = '            || v_checks_sys1
                                    || chr(13) || chr(10) || 'v_checks_mnp_sys2 = '         || v_checks_mnp_sys2
                                    || chr(13) || chr(10) || 'v_checks_mnp_sys3 = '         || v_checks_mnp_sys3
                                    || chr(13) || chr(10) || 'v_checks_mnp_sys1_new_req = ' || v_checks_mnp_sys1_new_req
                                    || chr(13) || chr(10) || 'v_checks = '                || v_checks);
    public.logs_p.write_detail_log('is_resend = ' || is_resend
                                     || chr(13) || chr(10) || 'in_date = ' || to_char(in_date, 'yyyymmdd hh24miss')
                                     || chr(13) || chr(10) || 'v_snap_date = ' || to_char(v_snap_date, 'yyyymmdd hh24miss')
                                     || chr(13) || chr(10) || 'in_rep_id = ' || in_rep_id
                                    );
```

### Courses:

- Introduction to HTML / Learn CSS in the [Codeacademy](https://www.codecademy.com/) (completed)<br>
- Frontend developer in [Netology](https://netology.ru/) (in progress) <br>
- Creating queries in Microsoft SQL Server 2012 based on the training center [Specialist](https://www.specialist.ru/) (completed)<br>

*********

### Languages:

- Russian - native speaker.
- English - B1 (B2 in process…)