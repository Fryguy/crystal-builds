FROM fryguy9/crystal:ruby

RUN git clone https://github.com/crystal-lang/crystal /opt/crystal-0.1.0 && \
    cd /opt/crystal-0.1.0 && \
    git checkout 0.1.0 && \
    rm -rf .git

RUN cd /opt/crystal-0.1.0 && \
    crystal --release -stats -o bin/crystal-exe src/compiler/crystal.cr
