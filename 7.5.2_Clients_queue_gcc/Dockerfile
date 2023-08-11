FROM ubuntu:16.04
	LABEL maintainer "surikovis89@gmail.com"
	RUN apt-get update && apt-get install -y build-essential nano
	WORKDIR /root/queue/
	COPY clients_queue.cpp .
	RUN g++ -std=c++11 -pthread clients_queue.cpp -o clients_queue
	CMD ["./clients_queue"]