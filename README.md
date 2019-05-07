# ![LOGO](logo.png) Open Skills **flow**ground Connector

## Description

A generated **flow**ground connector for the Open Skills API (version 1.0).

Generated from: https://api.apis.guru/v2/specs/dataatwork.org/1.0/swagger.json<br/>
Generated at: 2019-05-07T17:40:11+03:00

## API Description

A complete and standard data store for canonical and emerging skills, knowledge, abilities, tools, technolgies, and how they relate to jobs.

## Authorization

This API does not require authorization.

## Actions

### Job Titles and Descriptions

> Retrieves the names, descriptions, and UUIDs of all job titles.

#### Input Parameters
* `offset` - _optional_ - Pagination offset. Default is 0.
* `limit` - _optional_ - Maximum number of items per page. Default is 20 and cannot exceed 500.

### Job Title Autocomplete

> Retrieves the names, descriptions, and UUIDs of all job titles matching a given search criteria.

#### Input Parameters
* `begins_with` - _optional_ - Find job titles beginning with the given text fragment
* `contains` - _optional_ - Find job titles containing the given text fragment
* `ends_with` - _optional_ - Find job titles ending with the given text fragment

### Job Title Normalization

> Retrieves the canonical job title for a synonymous job title

#### Input Parameters
* `job_title` - _required_ - Find the canonical job title(s) for jobs matching the given text fragment
* `limit` - _optional_ - Maximumn number of job title synonyms to return. Default is 1 and cannot exceed 10.

### Unusual Job Titles

> Retrieves a list of unusual job titles and the UUIDs of their canonical jobs.

### Job Title and Description

> Retrieves the name, description, and UUID of a job by specifying its O*NET SOC Code or UUID.

#### Input Parameters
* `id` - _required_ - The O*NET SOC Code or UUID of the job title to retrieve
* `fips` - _optional_ - The FIPS Code of a Core-Based Statistical Area. Only return the job if present in this area

### Jobs Associated with a Job

> Retrieves a collection of jobs associated with a specified job.

#### Input Parameters
* `id` - _required_ - The UUID of the job to retrieve related jobs for

### Skills Associated with a Job

> Retrieves a collection of skills associated with a specified job.

#### Input Parameters
* `id` - _required_ - The UUID of the job to retrieve skills for

### Skill Names and Descriptions

> Retrieve the names, descriptions, and UUIDs of all skills.

#### Input Parameters
* `offset` - _optional_ - Pagination offset. Default is 0.
* `limit` - _optional_ - Maximum number of items per page. Default is 20 and cannot exceed 500.

### Skill Name Autocomplete

> Retrieves the names, descriptions, and UUIDs of all skills matching a given search criteria.

#### Input Parameters
* `begins_with` - _optional_ - Find skill names beginning with the given text fragment
* `contains` - _optional_ - Find skill names containing the given text fragment
* `ends_with` - _optional_ - Find skill names ending with the given text fragment

### Skill Name Normalization

> Retrieves the canonical skill name for a synonymous skill name

#### Input Parameters
* `skill_name` - _required_ - Find the canonical skill name(s) for skills matching the given text fragment

### Skill Name and Description

> Retrieves the name, description, and UUID of a job by specifying its UUID.

#### Input Parameters
* `id` - _required_ - The UUID of the skill name to retrieve

### Jobs Associated with a Skill

> Retrieves a collection of jobs associated with a specified skill.

#### Input Parameters
* `id` - _required_ - The UUID of the skill to retrieve jobs for

### Skills Associated with a Skill

> Retrieves a collection of skills associated with a specified skill.

#### Input Parameters
* `id` - _required_ - The UUID of the skill to retrieve related skills for

## License

**flow**ground :- Telekom iPaaS / dataatwork-org-connector<br/>
Copyright © 2019, [Deutsche Telekom AG](https://www.telekom.de)<br/>
contact: flowground@telekom.de

All files of this connector are licensed under the Apache 2.0 License. For details
see the file LICENSE on the toplevel directory.
