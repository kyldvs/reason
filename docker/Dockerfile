FROM ocaml/opam:debian
RUN sudo -u opam sh -c "opam switch 4.02.3"
RUN eval `opam config env`
RUN sudo -u opam sh -c "opam depext -u merlin utop"
RUN opam remote add main https://opam.ocaml.org && \
    opam install reason
