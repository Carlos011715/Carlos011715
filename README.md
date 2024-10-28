```java
public class GitHubProfile 
{
    private String name;
    private String interests;
    private String currentlyLearning;
    private String lookingFor;
    private String contactInfo;
    private String pronouns;
    private String funFact;
    private Socials socials;

    public GitHubProfile(String name, String interests, String currentlyLearning, String lookingToCollaborateOn, 
    String contactInfo, String pronouns, String funFact) 
    {
        this.name = name;
        this.interests = interests;
        this.currentlyLearning = currentlyLearning;
        this.lookingToCollaborateOn = lookingToCollaborateOn;
        this.contactInfo = contactInfo;
        this.pronouns = pronouns;
        this.funFact = funFact;
    }

    public String getName() {
        return name;
    }

    public String getInterests() {
        return interests;
    }

    public String getCurrentlyLearning() {
        return currentlyLearning;
    }

    public String getLookingToCollaborateOn() {
        return lookingToCollaborateOn;
    }

    public String getContactInfo() {
        return contactInfo;
    }

    public String getPronouns() {
        return pronouns;
    }

    public String getFunFact() {
        return funFact;
    }

    @Override
    public String toString() {
        return "GitHubProfile{" +
                "name='" + name + '\'' +
                ", interests='" + interests + '\'' +
                ", currentlyLearning='" + currentlyLearning + '\'' +
                ", lookingToCollaborateOn='" + lookingToCollaborateOn + '\'' +
                ", contactInfo='" + contactInfo + '\'' +
                ", pronouns='" + pronouns + '\'' +
                ", funFact='" + funFact + '\'' +
                '}';
    }

    public static void main(String [] args)
    {
        Socials socials = new Socials("mcarlitos1666@gmail.com", "www.linkedin.com/in/carlos-montero-jr17", "https://github.com/Carlos011715");

        GitHubProfile gitHubProfile = new GitHubProfile("Carlos Montero", "Programming and Pickleball", "Programming II and Discrete Structures", "anything", "Phone number - 305-336-3485", "He/Him", "I love Trading in the stock Market, instagram: Carlos0117");
    }
}

class Socials
{
    private String email;
    private String linkedin;
    private String github;

    public Socials(String email, String linkedin, String github) 
    {
        this.email = email;
        this.linkedin = linkedin;
        this.github = github;
    }

    public String getEmail() 
    {
        return email;
    }

    public String getLinkedin() 
    {
        return linkedin;
    }

    public String getGithub() 
    {
        return github;
    }

    @Override
    public String toString() 
    {
        return "Socials{" +
                "email='" + email + '\'' +
                ", linkedin='" + linkedin + '\'' +
                ", github='" + github + '\'' +
                '}';
    }
}
```