FROM jaegertracing/all-in-one@sha256:14a5e2ed08f458945d2067d9c51e23aaf23bbd2f68ffb1b22b0df1dcea970f6a
HEALTHCHECK \
    --interval=1s \
    --timeout=1s \
    --start-period=1s \
    --retries=60 \
    CMD wget -q --header='Content-Type:application/json' -O - http://localhost:14269/health | grep "Server available"
