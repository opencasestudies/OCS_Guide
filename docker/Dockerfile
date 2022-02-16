FROM jhudsl/course_template:main
LABEL maintainer="cwright60@jhu.edu"

# OCSData install
RUN R -e "options(warn = 2); install.packages(c('OCSdata'), \
  repos = 'https://cloud.r-project.org/')"
