<h1>Description:</h1>
<p>This is a Full-stack web development course for .NET 7.0 that I put together based on the resources available online for a study group I led about one year ago. Now publicly available and fully translated to English.</p>
<p>The purpose of this course is to structure the learning process so that you learn things in order and have all the knowledge necessary to follow to the next step.</p>
<p>While following the tutorials please have fun with the code and experiment with new tools instead of just watching or copying the code. It's vital for learning and understanding.</p>
<p>By the end of this course you should be fully equipt to create your own first project.</p>
<p>This course can be seperated into two overlapping sub-courses: one for Frontend and one for Backend.</p>
<h4>The full course is divided into 4 sub-sections:</h4>

<ul>
  <li><a href="#C">C#</a></li>
  <li><a href="#HTML&CSS">HTML & CSS</a></li>
  <li><a href="#CORE">ASP.NET Core</a></li>
  <li><a href="#BLAZOR">Blazor</a></li>
</ul>

<br>

<h4>Other technologies used/for you to explore:</h4>
<ul>
  <li>SQLite</li>
  <li>Git</li>
  <li>EF Core</li>
  <li>Xunit</li>
  <li>Mediatr</li>
  <li>MudBlazor</li>
  <li>Visual Studio 2022</li>
</ul>

<br>

<p>Disclaimer: I cannot guarantee that prepared materials will be available in the future nor that they will work on the newer releases of .NET, as I included the work of independent creators to which I have no affiliation. On this note, I would also like to credit them for their amazing work. They are doing the heavy lifting here, and I encourage you to check out their media for more useful content.</p>

<h2>Sub-courses:</h2>
<h3>Backend:</h3>
<ul>
  <li><a href="#C">C#</a></li>
  <li><a href="#CORE">ASP.NET Core</a></li>
</ul>
<h3>Frontend:</h3>
<ul>
  <li><a href="#C">C#</a></li>
  <li><a href="#HTML&CSS">HTML & CSS</a></li>
  <li><a href="#BLAZOR">Blazor</a></li>
</ul>
<br>




<h1 id="C">C#</h1>
<p>Welcome to the first part of the course. Here you will learn C#, which is a programming language that we will be using for the rest of the course.</p>

<h3>Why C#</h3>
<p>It's a general purpose languege developed by Microsoft. It was pupular in the backend development for quite a while now, and with Blazor gaining traction in Frontend there is no better time to learn it. By learning C#, we will also be able to learn the Full-stack with just one programming language, and by doing so, we will be able to focus more on the web-dev paradigms rather than on the language syntax.</p>

<h3>IDE instalation</h3>
<p>First we need to download the IDE. For that we will be using Visual Studio 2022</p>
<p><a href="https://visualstudio.microsoft.com/thank-you-downloading-visual-studio/?sku=Community&channel=Release&version=VS2022">https://visualstudio.microsoft.com/thank-you-downloading-visual-studio/?sku=Community&channel=Release&version=VS2022</a></p>
<p>Go through the instalation. Make sure to select the following:</p>
<ul>
  <li>ASP.NET and web development</li>
  <li>.NET desktop development</li>
  <li>.NET WebAssembly build tools</li>
  <li>Git for Windows</li>
</ul>

<img src="/images/1.png">
<img src="/images/2.png">
<img src="/images/3.png">
<img src="/images/4.png">

<h3>Coding</h3>
<p>Now we are ready to start coding. For that please follow the tutorial Bro Code made (big thanks) while also looking at the notes I will list below.</p>
<p>Link to the tutorial</p>
<p><a href="https://www.youtube.com/watch?v=r3CExhZgZV8&list=PLZPZq0r_RZOPNy28FDBys3GVP2LiaIyP_">https://www.youtube.com/watch?v=r3CExhZgZV8&list=PLZPZq0r_RZOPNy28FDBys3GVP2LiaIyP_</a></p>

<h3>Notes</h3>
<hr>
<p>Use <code>string</code> instead of <code>String</code></p>

<h4>Episode 5: Type casting</h4>
<p>Try to use Parse instead, as it allows for better debugging</p>
<pre><code>
string input = System.ReadLine();

// conversion string -> int with type safety
// public static bool TryParse(string s, out int result)
if (int.TryParse(input, out int number)
    Console.WriteLine("Valid number:" + number);
else
    Console.WriteLine("Invalid number");

// or:
// public static int Parse(string s)
int number2 = int.Parse(input);

// TryParse vs Parse:
// TryParse - returns true if the given text is a number and returns false otherwise. Number is stored in "out" variable.
// Parse - returns a number if conversion is possibly. Otherwise throwns an exception.
</code></pre>
<p>If the code above is unclear you can come back here after finishing all the videos.</p>

<h4>Episode 23: C# methods</h4>
<p>For naming methods use <code>PascalCase</code> instead of <code>camelCase</code>.</p>
<hr>

<h4>Bonus literature after watching all the videos. I would highly encourage you to read/watch the following to at least familiarize yourself with the tools at your disposal.</h4>
<p>Asynchronous programming (important!)</p>
<p><a href="https://www.youtube.com/watch?v=5a6WCBftjvw">https://www.youtube.com/watch?v=5a6WCBftjvw</a></p>
<p>Delegates</p>
<p><a href="https://learn.microsoft.com/en-us/dotnet/csharp/delegates-overview">https://learn.microsoft.com/en-us/dotnet/csharp/delegates-overview</a></p>
<p>Lambda expressions</p>
<p><a href="https://learn.microsoft.com/en-us/dotnet/csharp/language-reference/operators/lambda-expressions">https://learn.microsoft.com/en-us/dotnet/csharp/language-reference/operators/lambda-expressions</a></p>
<p>Access modifiers</p>
<p><a href="https://learn.microsoft.com/en-us/dotnet/csharp/programming-guide/classes-and-structs/access-modifiers">https://learn.microsoft.com/en-us/dotnet/csharp/programming-guide/classes-and-structs/access-modifiers</a></p>
<p>out</p>
<p><a href="https://learn.microsoft.com/en-us/dotnet/csharp/language-reference/keywords/method-parameters#out-parameter-modifier">https://learn.microsoft.com/en-us/dotnet/csharp/language-reference/keywords/method-parameters#out-parameter-modifier</a></p>
<p>IEnumerable&lt;T&gt;</p>
<p><a href="https://learn.microsoft.com/en-us/dotnet/api/system.collections.generic.ienumerable-1?view=net-7.0">https://learn.microsoft.com/en-us/dotnet/api/system.collections.generic.ienumerable-1?view=net-7.0</a></p>
<p>LINQ<T></p>
<pre><code>
// LINQ - Language Integrated Query - operations on collections
int[] nums = new int[] { 1, 1, 2, 3, 5, 8, 13, 21, 34 };
// LINQ operates on the IEnumerable<T> interface (or IQueryable<T>)
// LINQ is "lazy" - subsequent operations do not process data 
until the received collection is "materialized", e.g. by calling .ToArray()
// LINQ **does not** modify the original data

// Select - operation (in this case x * 2) on each element of the collection
int[] numsDoubled = nums.Select(x => x * 2).ToArray();

// Reverse - reverses the collection
int[] numsReversed = nums.Reverse().ToArray(); // or in this case .OrderByDescending(key => key)

// Where - returns the elements of the collection that meet the given condition
int[] numsEven = nums.Where(x => x % 2 == 0).ToArray();

// Distinct - distincs collection items
int[] numsUnique = nums.Distinct().ToArray();

// Skip - skips n elements
int[] nums2 = nums.Skip(5).ToArray(); // { 8, 13, 21, 34 }

// Take - returns n elements
int[] nums3 = nums.Take(5).ToArray(); // { 1, 1, 2, 3, 5 }

// Skip + Take
int[] nums4 = nums.Skip(3).Take(4).ToArray(); // { 3, 5, 8, 13 }

// Concat - appends another collection
int[] nums5 = nums.Concat(nums.Reverse()).ToArray(); 
// { 1, 1, 2, 3, 5, 8, 13, 21, 34, 34, 21, 13, 8, 5, 3, 2, 1, 1 }

// All/Any - checks whether all/any element meets the condition
bool allEven = nums.All(x => x % 2 == 0); // false
bool anyEven = nums.Any(x => x % 2 == 0); // true

int one = nums.First(); // = 1
int last = nums.Last(); // = 34
int sum2 = nums.Skip(1).Sum(); // = 87

// more: https://learn.microsoft.com/en-us/dotnet/api/system.linq.enumerable#methods
// there is "query syntax", it ends up using the same methods
</code></pre>
<p>Naming conventions</p>
<pre><code>
// Types - always PascalCase
internal class Program
{
	// Constants - always PascalCase
	public const int DefaultNumber = 0;

	// Properties - always PascalCase
	private int Number { get; } = 4;
	
	// private fileds - camelCase
	private int number2 = 3;

	// Methods - always PascalCase
	static void Main(string[] args /*parameters and variables - camelCase*/)
	{
		var program = new Program();
		program.number = program.Number;
	}
}

// Interfaces - I + PascalCase
public interface IXyz
{
	void DoXyz();
}

// Two-letter abbreviations - ALL CAPS
struct IPAddress
{
	public uint Value { get; }
}

// 3+ letter abbreviations - 1. big letter
struct MacAddress
{
	public ulong Value { get; }
}
</code></pre>




<h1 id="HTML&CSS">HTML & CSS</h1>
<h3>Coming to github soon</h3>

<h1 id="CORE">ASP.NET Core</h1>
<h3>Entry requirements</h3>
<ul>
  <li><a href="#C">C#</a></li>
</ul>

<p>Now, you are ready to learn how to apply your knowledge in practice. In this part of the course, we will focus on the Backend, which is a term used for the widely understood technical background of any application. Here in the server, all the stuff happens behind closed doors so that later Frontend (client) can display it to the user.</p>

<h3>What is ASP.NET Core</h3>
<p>ASP.NET Core is a framework for building web applications that utilizes C# and other .NET tools. It provides us with all the necessary tools and structure to easily build our own server-side application.</p>

<h3>Coding</h3>
<p>With that out of the way now we are ready to start coding. As before, please follow the tutorial Ervis Trupja made (big thanks) while also looking at the notes I will list below.</p>
<p>Link to the tutorial</p>
<p><a href="https://www.youtube.com/playlist?list=PL2Q8rFbm-4ru6hExDbfrN3QZNKI7n3p0N">https://www.youtube.com/playlist?list=PL2Q8rFbm-4ru6hExDbfrN3QZNKI7n3p0N</a></p>

<h3>Notes</h3>
<hr>
<h4>02. (Instalation)</h4>
<p>- skip it, you already have everything installed</p>

<h4>03. (New project)</h4>
<p>- sellect .NET 7.0 or newer and skip everything after 2:10</p>
<br>
<p>- to be able to follow the tutorial, which is in an older version, please paste the following as the program.cs</p>
<pre><code>
using Microsoft.AspNetCore.Hosting;
using System.Data.Common;
using <Project name>;
var builder = Host.CreateDefaultBuilder(args)
    .ConfigureWebHostDefaults(webBuilder =>
    {
        webBuilder.UseStartup<Startup>();
    });

builder.Build().Run();
</code></pre>

<p>- after that create a Startup.cs file and paste in the following:</p>
<pre><code>
using Microsoft.AspNetCore.Builder;
using Microsoft.EntityFrameworkCore;
using Microsoft.OpenApi.Models;
using System.Runtime;
using <Project name>.Data;
using <Project name>.Data.Services;
namespace <Project name>;

public class Startup
{
    public Startup(IConfiguration configuration)
    {
        Configuration = configuration;
    }

    public IConfiguration Configuration { get; }

    // This method gets called by the runtime. Use this method to add services to the container.
    public void ConfigureServices(IServiceCollection services)
    {


        // Add services to the container.

        services.AddControllers();

        // Learn more about configuring Swagger/OpenAPI at https://aka.ms/aspnetcore/swashbuckle
        services.AddEndpointsApiExplorer();
        services.AddSwaggerGen();

    }

    // This method gets called by the runtime. Use this method to configure the HTTP request pipeline.
    public void Configure(IApplicationBuilder app, IWebHostEnvironment env)
    {
        if (env.IsDevelopment())
        {
            app.UseSwagger();
            app.UseSwaggerUI();
        }

        app.UseHttpsRedirection();

        app.UseAuthorization();

        app.UseRouting();

        app.UseEndpoints(endpoints =>
        {
            endpoints.MapControllers();
        });
    }
}
</code></pre>

<p>Now it's important to note that we will be working on SQLite, as it provides free and lightweight experience while in the video tutorial MS SQL is the database of choice (which will be talked about all the time, so don't get confused)
Therefore, if you want to view your SQLite table in graphical form, install the following software:</p>
<p><a href="https://dbeaver.io/download/">https://dbeaver.io/download/</a></p>
<p>Then after creating your database (which we will be doing later) select that your Database is SQLite, provide the path to the file and, if necessary, install the additional files that will be suggested to you.
To view the data, select the table and then click the Data button or the ER Diagram button to view the relationships
When following tutorials, we always skip server explorer because we work on a different database, if you want to browse your database, use the linked software.</p>
<img id="ER" src="/images/5.png">

<h4>09. (DbContext)</h4>
<p>- (7:00) change <code>options.UseSqlServer(ConnectionString)</code> to <code>options.UseSqlite(ConnectionString)</code>
<p>- (7:45) change <code>Install-Package Microsoft.EntityFrameworkCore.SqlServer</code> to <code>Install-Package Microsoft.EntityFrameworkCore.Sqlite</code>

<h4>10. (Migration)</h4>
<p>- skip server explorer 1:30 - 2:30</p>
<p>- instead of that connection string <code>"Data Source=ETR"...</code> use <code>Data Source={}</code> and replace <code>{}</code> with the name of the (new) database file (e.g. test.db)</p>
<p>- the InitialDatabaseMigration class will be a little different, but it shouldn't have an inpact on this tutorial</p>
<p>- skip server explorer from 5:17</p>

<h4>11. (Seeding)</h4>
<p>- skip server explorer from 8:00</p>
<p>- this is not how you should seed a database, but still a good example of adding data to the db</p>

<h4>19. (One-to-Many)</h4>
<p>- skip server explorer from 6:00</p>

<h4>20. (Many-to-Many)</h4>
<p>- set navigation properties (<code>PublisherId</code> and <code>Publisher</code>) as optional (put a question mark after the type [<code>int? PublisherId</code> and <code>Publisher? Publisher</code>])</p>
<p>- skip server explorer 10:40 - 11:25</p>
<p>- if you want to make sure that you have the same relationships as in 11:30, go to the previously installed database software, select table for which you want to check the relationships and click the <a href="#ER">ER Diagram button</a></p>

<h4>21. (Adding Services)</h4>
<p>- skip server explorer from 13:10</p>

<h4>22. (Adding Relational Data)</h4>
<p>- skip server explorer 6:10 - 6:20 and from 9:00</p>

<h4>26. (Deleting Relational Data)</h4>
<p>- skip server explorer 3:53 - 4:25, 6:45 - 7:25, 7:50 - 8:30, 9:20 - 9:30, 9:50 - 10:10, 10:35+</p>
<p>- add new model Builder in AppDbContext:</p>
<pre><code>
modelBuilder.Entity<Book>()
  .HasOne(book => book.Publisher)
  .WithMany(pub => pub.Books)
  .HasForeignKey(book => book.PublisherId)
  .OnDelete(DeleteBehavior.Cascade);
</code></pre>
<p>- now build a new migration by entering <code>add-migration <name> in the Package Manager Console</code>.
After that, refresh the database by entering <code>update-database</code> in the same place</p>
<hr>

<h4>Bonus literature after watching all the videos. I would highly encourage you to read/watch the following to at least familiarize yourself with the tools at your disposal.</h4>
<p>Logger<T></p>
<p><a href="https://www.youtube.com/watch?v=NN9Rmf0PUG4&t=6s">https://www.youtube.com/watch?v=NN9Rmf0PUG4&t=6s</a></p>
<p>Status codes</p>
<p><a href="https://learn.microsoft.com/en-us/dotnet/api/microsoft.aspnetcore.http.statuscodes?view=aspnetcore-8.0">https://learn.microsoft.com/en-us/dotnet/api/microsoft.aspnetcore.http.statuscodes?view=aspnetcore-8.0</a></p>
<p>Headers</p>
<p><a href="https://learn.microsoft.com/en-us/dotnet/api/system.net.http.headers.httpheaders.add?view=net-8.0">https://learn.microsoft.com/en-us/dotnet/api/system.net.http.headers.httpheaders.add?view=net-8.0</a></p>
<p>Authorization</p>
<p><a href="https://learn.microsoft.com/en-us/aspnet/core/security/authorization/introduction?view=aspnetcore-8.0">https://learn.microsoft.com/en-us/aspnet/core/security/authorization/introduction?view=aspnetcore-8.0</a></p>

<p>You are now done with the theory for Backend course. All that's left for you to do now is a one final project to test your skills in practice</p>

<h2>Final Project</h2>
<p>Write a program using the newest version of .NET (without creating a startup.cs file) that:</p>
<p>- will use SQLite</p>
<p>- will have two tables in the database: "Languages" and "Programmers"</p>
<p>- Languages ​​has fields: ID, Name, Programmers</p>
<p>- Programmers has fields: ID, FullName, JoinDate(date added), LeaveDate(optional), Languages</p>
<p>- then add a mana-to-many relationship between the previous two arrays</p>
<p>- create the following endpoints (the names may differ slightly):</p>
<p>- for Languages:</p>
<pre><code>
DELETE /api/languages/{id}
POST /api/languages
GET /api/languages
PUT /api/languages/{id}
GET /api/languages/{id}/programmers
</code></pre>
<p>- for Programmers:</p>
<pre><code>
DELETE /api/programmers/{id}
POST /api/programmers
GET /api/programmers
PUT /api/programmers/{id}
GET /api/programmers/{id}/languages
</code></pre>


<p>- finally, add yourself to the database in the Programmers table and the appropriate programming languages ​​that match you in the Languages ​​table, as well as one other person (can be made up) whose at least one language will overlap with yours</p>

<h4>After you are done with your project, or if you get really stuck you can compare your code to mine</h4>
<p><a href="/code/ASP.NET_Core-final_project/">My code</a></p>
<hr>


<h1 id="BLAZOR">Blazor</h1>
<h3>Coming to github soon</h3>


