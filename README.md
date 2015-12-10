Summary
-------

Chronograf server image. Chronograf is a web application for exploring time series
data stored in a InfluxDB database.


Build the image
---------------

To create this image, execute the following command in the docker-chronograf folder.

    docker build -t cburki/chronograf .


Run the image
-------------

The chronograf HTTP server is listening on port 10000 so we bind this port when
running the container.

    docker run \
        --name chronograf \
        -p 10000:10000 \
        -d \
        cburki/chronograf:latest
