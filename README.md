# Spring-Data-JPA--Testing-Project-using-DataJPATest
SpringData-JPA-Test project to gain knowledge how to do Unit Testing on DB using JPAtest
# prerequisite
1. JDK 8 
2. Maven 3.3.x
3. 
#Instruction & Details to Run this project

1. Download the zip file & extract in some location
2. Import any IDE( Eclipse/IntelliJ) as a Existing Maven Project
3. Build the project by selecting -> "maven Install" ( command line : mvn clean install )
4. finally run by -> "maven Test"  ( command line : mvn test )

#Youtube Video Link : 


#Details

@DataJpaTest is the annotation that Spring supports for a JPA test that focuses only on JPA components.

It will disable full auto-configuration and then, apply only enable configuration relevant to JPA tests. The list of the auto-configuration settings that are enabled can be found here.

By default, tests annotated with @DataJpaTest are transactional and roll back at the end of each test. If you don’t want it, you can disable transaction management for a test or for the whole class using @Transactional annotation:

The purpose of the EntityManager is to interact with the persistence context. Spring Data JPA abstractes you from the EntityManager through Repository interfaces. And TestEntityManager allows us to use EntityManager in tests.

We can inject a TestEntityManager bean in Data JPA tests. If you want to use TestEntityManager outside of @DataJpaTest instances, just add @AutoConfigureTestEntityManager annotation.
