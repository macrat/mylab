FROM afian/filerun

RUN groupadd -g 1000 filerun && useradd -u 1000 -g filerun filerun
RUN chown filerun:filerun -R /user-files /var/www
RUN sed -i -e 's/www-data/filerun/g' /entrypoint.sh

ENV APACHE_RUN_USER filerun
ENV APACHE_RUN_GROUP filerun
