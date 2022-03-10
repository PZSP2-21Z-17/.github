# Exam Paper Manager

or, more verbosely, Exam Paper Generation and Archivization System.

A project for [Team Project 2](https://usosweb.usos.pw.edu.pl/kontroler.php?_action=katalog2%2Fprzedmioty%2FpokazPrzedmiot&prz_kod=103A-INxxx-ISP-PZSP2&lang=en) course on WUT.

## Main features

* support for multiple choice closed-ended questions (tasks) only    
  (there is no required number of correct answers or answers at all – this enables emulation of single choice and open-ended questions as well)
* simple authentication and authorization    
  (users can set created tasks either as public or private, ie. visible for others or not)
* division of tasks into categories using mandatory subjects (one per task) and optional tags
* task search based on assigned subject, tasks and content (using trigrams)
* support for HTML, Markdown and LaTeX in task content
* client-side preview and PDF generation
* possibility of answer sheet generation (for easier marking)
* generation of multiple test groups sharing a task pool, but sampled randomly
* automatic archivization of generated exam papers

## Tech stack

1. Presentation Tier
    * **TypeScript**
    * React – designing user views
    * Bootstrap – user-friendly interface styling
    * Jest – unit testing

2. Logic Tier
    * **Python**
    * FastAPI – providing a REST interface
    * SQLAlchemy – interacting with the database
    * pytest – unit testing

3. Data Tier
    * **PostgreSQL**

## Quick setup

Check out the umbrella repository for details:  
https://github.com/PZSP2-21Z-17/docker-compose
