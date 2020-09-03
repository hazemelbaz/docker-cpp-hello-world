FROM gcc:8.2 as builder
COPY . /myapp
WORKDIR /myapp
RUN g++ -o myapp -static hello.cpp

FROM alpine:latest
COPY --from=builder /myapp/myapp /myapp
# TODO would be better to not run the app as root...
CMD ["./myapp"]