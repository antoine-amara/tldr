# pprof

> Comand-line tool for visualization and analysis of profiling data.
> More information: <https://github.com/google/pprof>.

- Generate a text report from fibbo-profile.pb.gz profile data on fibbo binary:

`pprof -top {{./fibbo}} {{./fibbo-profile.pb.gz}}`

- Generate a graph from fibbo-profile.pb.gz profile data and open it on a web browser:

`pprof -svg {{./fibbo}} {{./fibbo-profile.pb.gz}}`

- Run pprof on interactive mode and customize your report with pprof command:

`pprof {{./fibbo}} {{./fibbo-profile.pb.gz}}`

- Run a web server to have a web interface on top of pprof:

`pprof -http={{localhost:8080}} {{./fibbo}} {{./fibbo-profile.pb.gz}}`

- Fetch a profile from an HTTP server and generate a report:

`pprof {{http://localhost:8080/debug/pprof/profile}}`
