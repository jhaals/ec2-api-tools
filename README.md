# Create ec2-api-tools debian package
`create_ec2_api_tools_deb` downloads the latest version from amazon and builds a debian package that install the tools in `/opt/ec2-api-tools`. unzip and fpm is required to build the package.

This custom build is solely because [ppa:awstools-dev/awstools](https://launchpad.net/~awstools-dev/+archive/ubuntu/awstools) is outdated

Required environment variables

    export AWS_ACCESS_KEY=your-aws-access-key-id
    export AWS_SECRET_KEY=your-aws-secret-key
    export JAVA_HOME="/path/to/java_home/"
    export EC2_HOME="/opt/ec2-api-tools"
