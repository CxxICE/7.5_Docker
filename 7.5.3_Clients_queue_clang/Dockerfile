FROM ubuntu:16.04
	LABEL maintainer "surikovis89@gmail.com"
	RUN apt-get update && apt-get install -y clang nano
	WORKDIR /root/hello/
	COPY clients_queue.cpp .
	RUN clang++ -pthread -std=c++11 clients_queue.cpp -o clients_queue
	CMD ["./clients_queue"]