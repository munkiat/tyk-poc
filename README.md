# **Tyk Self-Managed Trial using Docker**

# **Quick start**

### **Prerequisites**

* Install Docker (Docker Engine 20.10.0 or newer)  
* Install the following CLI tools:  
  * git (for cloning GitHub repositories)  
  * curl (for making API requests)  
* Get a Tyk Self-Managed license key (see below)

### **Getting a License**

Use the license key sent to you when you signed up for your self-managed trial.

* Don’t have a license? [Sign up here](https://tyk.io/self-managed-trial)  
* Signed up but didn’t receive your key? Contact [info@tyk.io](mailto:info@tyk.io)  
* License expired? [Contact us to discuss an extension](https://tyk.io/contact/)

### **Deploying Tyk**

Clone the repository:

```
git clone https://github.com/TykTechnologies/tyk-self-managed-trial && cd tyk-self-managed-trial
```

Create a `.env` file in the root directory with the following:

```
DASH_LICENSE=<your-tyk-license-key>
```

Use `.env.example` as a reference if needed.

Start the Tyk stack:

```
docker compose up -d
```

Verify that all containers are running:

```
docker compose ps
```

**Accessing your Tyk installation** 

```
---------------------------
Your Tyk Dashboard URL is http://localhost:3000

user: developer@tyk.io
pw: specialpassword
---------------------------
Your Tyk Gateway URL is http://localhost:8080
---------------------------
Your Developer Portal URL is http://localhost:3001

admin user: portaladmin@tyk.io
admin pw: specialpassword
---------------------------
```

### **Cleaning Up Docker Containers** 

To stop and remove containers and volumes:

```
docker compose down -v
```

### **Need help?** 

* **Didn’t receive your license key?** Please contact info@tyk.io

* **License expired?** [Contact us to discuss options for extending your trial](https://tyk.io/contact/)

* **Need technical support:** Trial users can use the [Tyk self-managed](https://tyk.io/docs/tyk-self-managed/) documentation and [Community Forum](https://community.tyk.io/). Direct support is not included during the trial.

* **Looking for a guided Proof of Concept?** [Get in touch for more information.](https://tyk.io/guided-evaluation/)   
    
* **Got other questions?** Please email info@tyk.io  
  
