FROM openjdk:8

WORKDIR /src/java

RUN echo "class Hello{public static void main(String args[]){System.out.println(\"Hello Java\");}} " > Hello.java

RUN ["javac","Hello.java"]

ENTRYPOINT ["java","Hello"]

# docker build -t 04 . && docker run -it 04