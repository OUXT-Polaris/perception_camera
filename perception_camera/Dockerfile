FROM perception_camera_perseption_camera

RUN apt-get update && \
    apt-get install -y --no-install-recommends \
    libzmqpp-dev && \
    apt-get -y clean  && \
    rm -rf /var/lib/apt/lists/*
ADD https://api.github.com/repos/OUXT-Polaris/perception_camera_app/git/refs/heads/master version.json
RUN git clone -b master https://github.com/OUXT-Polaris/perception_camera_app.git /root