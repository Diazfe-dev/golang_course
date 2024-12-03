# ---------------------
# general formats
# ---------------------

# 1. build input file "filename.go" into an executable
# named "executable_filename" within the directory you are currently `cd`ed
# into
go build -o executable_filename filename.go

# 2. build input file "filename.go" into an executable at
# path "output_dir/filename"; this automatically creates directory "output_dir"
# if it does not already exist (don't forget the trailing slash after the
# directory name!)
go build -o output_dir/ filename.go

# 3. build input file "filename.go" into an executable at
# path "output_dir/whatever"; this automatically creates directory "output_dir"
# if it does not already exist
go build -o output_dir/whatever filename.go

# ---------------------
# examples
# ---------------------

# create executable "whatever" from "hello_world.go"
go build -o whatever hello_world.go

# make directory "bin" and create executable "bin/hello_world"
# from "hello_world.go"
go build -o bin/ hello_world.go

# make directory "bin" and create executable "bin/whatever"
# from "hello_world.go"
go build -o bin/whatever hello_world.go

# ---------------------
# help
# ---------------------

# see the short help menu for `go build`
go build --help

# see the long help menu for `go build`
go help build