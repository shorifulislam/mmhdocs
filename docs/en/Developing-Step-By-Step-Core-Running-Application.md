# Running the Application

**It's finished**! We can test the application. Run the project, **login** as the **host admin** (click Change link and clear tenancy name) shown below:

<img src="images/login-as-host-5.png" alt="Login as host" class="img-thumbnail" />

Default **admin** password is **123qwe**. After login, we see the **tenant list** which only contains a **default** tenant. We can create a new tenant:

<img src="images/create-tenant-7.png" alt="Creating tenant" class="img-thumbnail" />

I created a new tenant named **trio**. Now, tenant list has two tenants:

<img src="images/tenant-list-with-2-tenant-2.png" alt="Tenant list" class="img-thumbnail" />

I can **logout** and login as **trio** tenant **admin** (Change current tenant to trio):

<img src="images/login-as-trio3.png" alt="Login as tenant admin" class="img-thumbnail" />

After login, we see that phone book is empty:

<img src="images/phonebook-empty2.png" alt="Empty phonebook of new tenant" class="img-thumbnail" />

It's empty because trio tenant has a completely isolated people list.
You can add people here, logout and login as different tenants (you can
login as default tenant for example). You will see that each tenant has
an isolated phone book and can not see other's people.

## Next

- [Conclusion](Developing-Step-By-Step-Core-Conclusion.md)