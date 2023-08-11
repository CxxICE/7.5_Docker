FROM ubuntu:16.04
	LABEL maintainer "surikovis89@gmail.com"
	RUN apt-get update && apt-get install -y g++ nano
	WORKDIR /root/hello/
	COPY hello.cpp .
	RUN g++ hello.cpp -o hello
	CMD ["./hello"]