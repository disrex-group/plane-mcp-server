# Changelog

All notable changes to the Plane MCP Server will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [0.4.0] - 2025-01-16

### Added

#### Issue Property Management (8 tools)
- `list-issue-properties` - List all custom properties for a specific issue type
- `get-issue-property` - Get details of a specific issue property
- `create-issue-property` - Create a new custom property for an issue type
- `update-issue-property` - Update an existing issue property
- `delete-issue-property` - Delete an issue property
- `list-issue-property-options` - List all options for a dropdown/select issue property
- `create-issue-property-option` - Create a new option for a dropdown/select issue property
- `update-issue-property-option` - Update an option for a dropdown/select issue property

#### Sub-issues & Relations (4 tools)
- `list-sub-issues` - List all sub-issues of a parent issue
- `create-sub-issue` - Create a new sub-issue under a parent issue
- `convert-to-sub-issue` - Convert an existing issue to a sub-issue of another issue
- `convert-to-issue` - Convert a sub-issue back to a regular issue (remove parent relationship)

#### Issue Transfer Operations (1 tool)
- `transfer-issues` - Transfer issues from one cycle to another

### Changed
- Expanded tool count from 63 to 76 tools total (13 new tools)
- Updated package description to reflect comprehensive feature set
- Added keywords for new functionality (custom-properties, sub-issues, relations, transfer)

### Documentation
- Updated CHANGELOG with detailed feature additions
- Enhanced package metadata to reflect expanded capabilities

## [0.3.0] - 2025-01-16

### Added

#### Issue Comments (5 tools)
- `list-issue-comments` - List all comments for an issue
- `get-issue-comment` - Get a specific comment by ID
- `create-issue-comment` - Create a new comment on an issue
- `update-issue-comment` - Update an existing comment
- `delete-issue-comment` - Delete a comment

#### Issue Links (5 tools)
- `list-issue-links` - List all links for an issue
- `get-issue-link` - Get a specific link by ID
- `create-issue-link` - Create a new link between issues
- `update-issue-link` - Update an existing link
- `delete-issue-link` - Delete a link

#### Issue Attachments (2 tools)
- `list-issue-attachments` - List all attachments for an issue
- `delete-issue-attachment` - Delete an attachment

#### Issue Activities (2 tools)
- `list-issue-activities` - List all activities for an issue
- `get-issue-activity` - Get a specific activity by ID

#### Time Tracking & Worklogs (5 tools)
- `list-issue-worklogs` - List all time logs for an issue
- `get-issue-worklog` - Get a specific worklog by ID
- `create-issue-worklog` - Create a new time log entry
- `update-issue-worklog` - Update an existing worklog
- `delete-issue-worklog` - Delete a worklog

#### Issue Types (5 tools)
- `list-issue-types` - List all issue types in workspace
- `get-issue-type` - Get a specific issue type by ID
- `create-issue-type` - Create a new issue type
- `update-issue-type` - Update an existing issue type
- `delete-issue-type` - Delete an issue type

#### Intake Issues (5 tools)
- `list-intake-issues` - List all intake issues for a project
- `get-intake-issue` - Get a specific intake issue by ID
- `create-intake-issue` - Create a new intake issue
- `update-intake-issue` - Update an existing intake issue
- `delete-intake-issue` - Delete an intake issue

### Changed
- Updated package name from `@disrex-group/plane-mcp-server` to `@disrex/plane-mcp-server` to match npm organization
- Expanded tool count from 32 to 63 tools total
- Enhanced package description to reflect comprehensive feature set
- Added keywords for new functionality (comments, attachments, time-tracking, worklogs, issue-types, intake, links)

### Fixed
- Corrected API key generation instructions in README (personal settings vs workspace settings)
- Added cloud-only compatibility warning for Plane instances
- Removed package-lock.json from .gitignore to fix GitHub Actions CI
- Filled in all missing tool examples in README documentation

### Documentation
- Added comprehensive examples for all 31 new tools
- Updated README with proper API key generation instructions
- Added cloud instance compatibility requirements
- Enhanced tool descriptions with detailed parameter explanations

## [0.2.0] - 2025-01-15

### Added
- Initial MCP server implementation with 32 core tools
- Project management (projects, members, favorites)
- Issue management (CRUD operations, assignments, subscribers)
- Sprint/Cycle management
- Label and state management
- Module management
- View management
- Basic workspace operations

## [0.1.0] - 2025-01-14

### Added
- Initial project setup
- Basic TypeScript configuration
- MCP SDK integration
- Core project structure