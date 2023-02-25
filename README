# Scandium

This is a JavaScript code implementing an Access Control List (ACL) system. ACL is a security model that defines access rights and permissions for users or roles to access specific resources or perform certain actions. The code defines an ACL object that contains methods for adding roles, resources, and rules, as well as methods for checking if a user or role has access to a resource or action.

# Specification
## Roles

    - A role is an identifier that represents a group of users with similar permissions.
    - A role can be assigned to one or more users.
    - A role can inherit permissions from another role.
    - A role can have one or more parent roles.

## Resources

    - A resource is an identifier that represents a system resource or an action.
    - A resource can be a URL, file, or any other system object.
    - A resource can have one or more permissions.
    - A resource can be accessed by one or more roles.

## Permissions

    - A permission is an identifier that represents a system action that can be performed on a resource.
    - A permission can be granted or denied for a role on a resource.
    - A permission can be allowed or denied based on a condition.

## ACL API

The ACL implementation should provide the following API:

    - addRole(role: Role, parentRole?: Role): void - adds a role to the ACL with an optional parent role.
    - addResource(resource: Resource): void - adds a resource to the ACL.
    - allow(permission: string, resource: string, role: string, condition?: Condition): void - allows a permission on a resource for a role with an optional condition.
    - deny(permission: string, resource: string, role: string, condition?: Condition): void - denies a permission on a resource for a role with an optional condition.
    - isAllowed(permission: string, resource: string, role: string, params?: any[]): boolean - checks if a role is allowed to perform a permission on a resource with optional parameters.
    - getRole(roleName: string): Role - retrieves a role from the ACL.
    - getResource(resourceName: string): Resource - retrieves a resource from the ACL.

## Role API

The Role object should provide the following API:

    - addParentRole(parentRole: Role): void - adds a parent role to the role.
    - getPermissions(): Permission[] - retrieves all the permissions for the role.
    - getRoleName(): string - retrieves the name of the role.

## Resource API

The Resource object should provide the following API:

    - addPermission(permission: Permission): void - adds a permission to the resource.
    - getPermissions(): Permission[] - retrieves all the permissions for the resource.
    - getResourceName(): string - retrieves the name of the resource.

## Permission API

The Permission object should provide the following API:

    - getPermissionName(): string - retrieves the name of the permission.
    - isAllowed(params?: any[]): boolean - checks if the permission is allowed with optional parameters.
    - getCondition(): Condition - retrieves the condition for the permission if it exists.

## Condition API

The Condition object should provide the following API:

    - evaluate(params?: any[]): boolean - evaluates the condition with optional parameters.
