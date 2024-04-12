# Reddit-Data-Analysis
This project is to provide an analysis and visualize a social media graph corresponding to Reddit.

<h2>Introduction</h2>
<p>
The purpose of this project was to gather data from social media and compile it into a dataset. We were
also required to search for, examine, and visualize the data using graphs. After that, we had to provide
the retrieved data for a new analysis. Reddit was our social media platform of choice for obtaining the
necessary data
</p>

<h2>Insights from Results</h2>
<p>The analysis of the Reddit social network graph has provided several insights into user interactions
and network dynamics within the platform. By leveraging NetworkX for graph construction and measurement, we were able to explore key metrics such as Degree Distribution, Closeness Centrality, and PageRank.</p><br>
<p>Degree Distribution: The presence of a large number of zero or nearly zero weights, indicating
minimal or no shared subreddits between certain users, contributed to the complexity of the network by
increasing the number of edges. The weights ranged from 2 to 170, requiring eventual scaling down and
normalization.</p>
<p>The right-skewed distribution suggests that while there are a few highly connected users (nodes) with a
high number of subreddits (edges), the majority of users have lower degrees. This indicates a hierarchical
structure within the network where a small number of users potentially hold significant influence or act
as connectors.</p><br>
<p>Closeness Centrality: Nodes with higher closeness centrality scores are more central within the network, indicating their proximity to other nodes. This suggests that certain users may have a higher potential to disseminate information or influence others due to their central position in the network.</p><br>
<p>PageRank: Users with higher PageRank scores are likely to have a wider reach and influence within the
network. These users may serve as important starting points for information diffusion and are crucial in
predicting how trends or information spread throughout the community.</p>


<h3>Code Details</h3>
<p>The src/ folder contains files as follows :
 <ul>- parser.ipynb </ul>
 <ul>- graph_viz.ipynb</ul>
 <ul>- config.json</ul>
 <ul>- user_activity.json</ul>
</p><br>
<p>To run this project, please follow the below instructions:<br>
    <ul>1. We have used jupyter notebook for development, if not available kindly install using pip (pip install notebook).</ul>
    <ul>2. To run the project, we need to install the necessary libraries mentioned in the 'requirements.txt'. For ease, you can run using "pip install -r requirements.txt"</ul>
    <ul>3. The first part of the project is reading and parsing Reddit Data, which is provided in the 'parser.ipynb' which requires Reddit Dev Credentials specified in the 'config.json'.</ul>
    <ul>4. The 'parser.ipynb' at the end generates an json file (used for intermittent storage) (can take about 6-7 minutes), further used for graph visualization. We have provided a sample json for usage.</ul>
    <ul>5. The 'graph_viz.ipynb' file is used for graph visualization. The 'Pyvis' library is utilized for visualization and it generates a separate html file named as 'nx.html' which displays the network graph (takes 1-2 minutes to render the graph). The file also contains the network measures such as closeness centrality, degree distribution as well as page rank.</ul></p>
