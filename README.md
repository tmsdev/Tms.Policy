# Tms.Policy

Nodetype mixins for common privilege tasks in your Neos CMS setup.

**Why would I need mixins for that?** Keeping the number of privilege targets as low as possible can boost your Neos backend performance.

## Install

```bash
composer require tms/policy
```

## Usage

```yaml
'Your.Package:Type':
  superTypes:
    'Tms.Policy:Mixin.Privilege.CreateNode': true
    'Tms.Policy:Mixin.Privilege.RemoveNode': true
```

This configuration allows only `Administrator` roles to create and/or remove node of type `Your.Package:Type`. Feel free to adjust the policy settings to your needs.

## Acknowledgments

Development sponsored by [tms.development - Online Marketing and Neos CMS Agency](https://www.tms-development.de/)
