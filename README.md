# ansible-role-awslogs

## Description

Amazon EC2 Scripts to run Amazon CloudWatch Logs as a daemon.

## Requirements

None

## Dependencies

None

## OS Platforms

- AmazonLinux-2

## Example Playbook

```yaml
- hosts: all
  roles:
    - awslogs
```

## Role Variables

### awslogs_debug

```yaml
awslogs_debug: false
```

### awslogs_package_ensure: (string)

```yaml
awslogs_package_ensure: present
```

### awslogs_service_name: (string)

```yaml
awslogs_service_name: 'awslogsd'
```

### awslogs_service_ensure: (string)

```yaml
awslogs_service_ensure: 'started'
```

### awslogs_service_enable: (bool)

```yaml
awslogs_service_enable: true
```

### awslogs_config_options: (dict)

None

### awslogs_cli_config_options: (dict)

None

### awslogs_proxy_config_options: (dict)

None

### awslogs_dropin_config_options: (dict)

None

## Example vars

```yaml
awslogs_cli_config_options:
    default:
      region: 'ap-northeast-1'
```
