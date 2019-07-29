FROM ubuntu
RUN apt-get update
RUN apt-get install -y build-essential
COPY hello.c /
RUN make hello
CMD /hello
FROM ubuntu 
COPY --from=0 /hello /hello 
CMD /hello
