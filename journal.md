mkdir td5_docker_runner_web_php_bdd
scp -r  simplephpdb20231030_074447/* docker:/home/user/ci_cd_dajani_amir_trabelsi/td5_docker_runner_web_php_bdd/
cd td5_docker_runner_web_php_bdd
nano docker-compose.yml
nano journal.md
nano index.php # config a la connexion a la base de donné la ligne  $pdo = new PDO("mysql:dbname=td_docker_runner_bdd;host=mariadb", "root", "");
docker compose up -d
