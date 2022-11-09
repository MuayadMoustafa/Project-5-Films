```python
import pandas as pd 
```


```python
df = pd.read_excel("C:/Users/Mua/Downloads/film.xlsx")
df
```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>Year</th>
      <th>Length</th>
      <th>Title</th>
      <th>Subject</th>
      <th>Actor</th>
      <th>Actress</th>
      <th>Director</th>
      <th>Popularity</th>
      <th>Awards</th>
      <th>*Image</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>INT</td>
      <td>INT</td>
      <td>STRING</td>
      <td>CAT</td>
      <td>CAT</td>
      <td>CAT</td>
      <td>CAT</td>
      <td>INT</td>
      <td>BOOL</td>
      <td>STRING</td>
    </tr>
    <tr>
      <th>1</th>
      <td>1990</td>
      <td>111</td>
      <td>Tie Me Up! Tie Me Down!</td>
      <td>Comedy</td>
      <td>Banderas, Antonio</td>
      <td>Abril, Victoria</td>
      <td>False</td>
      <td>68</td>
      <td>No</td>
      <td>NicholasCage.png</td>
    </tr>
    <tr>
      <th>2</th>
      <td>1991</td>
      <td>113</td>
      <td>High Heels</td>
      <td>Comedy</td>
      <td>False</td>
      <td>Abril, Victoria</td>
      <td>False</td>
      <td>68</td>
      <td>No</td>
      <td>NicholasCage.png</td>
    </tr>
    <tr>
      <th>3</th>
      <td>1983</td>
      <td>104</td>
      <td>Dead Zone, The</td>
      <td>Horror</td>
      <td>Walken, Christopher</td>
      <td>Adams, Brooke</td>
      <td>Cronenberg, David</td>
      <td>79</td>
      <td>No</td>
      <td>NicholasCage.png</td>
    </tr>
    <tr>
      <th>4</th>
      <td>1979</td>
      <td>122</td>
      <td>Cuba</td>
      <td>Action</td>
      <td>Connery, Sean</td>
      <td>Adams, Brooke</td>
      <td>Lester, Richard</td>
      <td>6</td>
      <td>No</td>
      <td>seanConnery.png</td>
    </tr>
    <tr>
      <th>...</th>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
    </tr>
    <tr>
      <th>1655</th>
      <td>1932</td>
      <td>226</td>
      <td>Shadow of the Eagle, The</td>
      <td>Action</td>
      <td>Wayne, John</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>19</td>
      <td>No</td>
      <td>johnWayne.png</td>
    </tr>
    <tr>
      <th>1656</th>
      <td>1989</td>
      <td>103</td>
      <td>Blood &amp; Guns</td>
      <td>Action</td>
      <td>Welles, Orson</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>43</td>
      <td>No</td>
      <td>NicholasCage.png</td>
    </tr>
    <tr>
      <th>1657</th>
      <td>1988</td>
      <td>78</td>
      <td>Hot Money</td>
      <td>Drama</td>
      <td>Welles, Orson</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>19</td>
      <td>No</td>
      <td>NicholasCage.png</td>
    </tr>
    <tr>
      <th>1658</th>
      <td>1977</td>
      <td>75</td>
      <td>Comedy Tonight</td>
      <td>Comedy</td>
      <td>Williams, Robin</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>18</td>
      <td>No</td>
      <td>NicholasCage.png</td>
    </tr>
    <tr>
      <th>1659</th>
      <td>1991</td>
      <td>65</td>
      <td>Robin Williams</td>
      <td>Comedy</td>
      <td>Williams, Robin</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>4</td>
      <td>No</td>
      <td>NicholasCage.png</td>
    </tr>
  </tbody>
</table>
<p>1660 rows × 10 columns</p>
</div>




```python
dff = df.head(50)
dff
```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>Year</th>
      <th>Length</th>
      <th>Title</th>
      <th>Subject</th>
      <th>Actor</th>
      <th>Actress</th>
      <th>Director</th>
      <th>Popularity</th>
      <th>Awards</th>
      <th>*Image</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>INT</td>
      <td>INT</td>
      <td>STRING</td>
      <td>CAT</td>
      <td>CAT</td>
      <td>CAT</td>
      <td>CAT</td>
      <td>INT</td>
      <td>BOOL</td>
      <td>STRING</td>
    </tr>
    <tr>
      <th>1</th>
      <td>1990</td>
      <td>111</td>
      <td>Tie Me Up! Tie Me Down!</td>
      <td>Comedy</td>
      <td>Banderas, Antonio</td>
      <td>Abril, Victoria</td>
      <td>False</td>
      <td>68</td>
      <td>No</td>
      <td>NicholasCage.png</td>
    </tr>
    <tr>
      <th>2</th>
      <td>1991</td>
      <td>113</td>
      <td>High Heels</td>
      <td>Comedy</td>
      <td>False</td>
      <td>Abril, Victoria</td>
      <td>False</td>
      <td>68</td>
      <td>No</td>
      <td>NicholasCage.png</td>
    </tr>
    <tr>
      <th>3</th>
      <td>1983</td>
      <td>104</td>
      <td>Dead Zone, The</td>
      <td>Horror</td>
      <td>Walken, Christopher</td>
      <td>Adams, Brooke</td>
      <td>Cronenberg, David</td>
      <td>79</td>
      <td>No</td>
      <td>NicholasCage.png</td>
    </tr>
    <tr>
      <th>4</th>
      <td>1979</td>
      <td>122</td>
      <td>Cuba</td>
      <td>Action</td>
      <td>Connery, Sean</td>
      <td>Adams, Brooke</td>
      <td>Lester, Richard</td>
      <td>6</td>
      <td>No</td>
      <td>seanConnery.png</td>
    </tr>
    <tr>
      <th>5</th>
      <td>1978</td>
      <td>94</td>
      <td>Days of Heaven</td>
      <td>Drama</td>
      <td>Gere, Richard</td>
      <td>Adams, Brooke</td>
      <td>Malick, Terrence</td>
      <td>14</td>
      <td>No</td>
      <td>NicholasCage.png</td>
    </tr>
    <tr>
      <th>6</th>
      <td>1983</td>
      <td>140</td>
      <td>Octopussy</td>
      <td>Action</td>
      <td>Moore, Roger</td>
      <td>Adams, Maud</td>
      <td>Glen, John</td>
      <td>68</td>
      <td>No</td>
      <td>NicholasCage.png</td>
    </tr>
    <tr>
      <th>7</th>
      <td>1984</td>
      <td>101</td>
      <td>Target Eagle</td>
      <td>Action</td>
      <td>Connors, Chuck</td>
      <td>Adams, Maud</td>
      <td>False</td>
      <td>14</td>
      <td>No</td>
      <td>NicholasCage.png</td>
    </tr>
    <tr>
      <th>8</th>
      <td>1989</td>
      <td>99</td>
      <td>American Angels: Baptism of Blood, The</td>
      <td>Drama</td>
      <td>Bergen, Robert D.</td>
      <td>Adams, Trudy</td>
      <td>Sebastian, Beverly</td>
      <td>28</td>
      <td>No</td>
      <td>NicholasCage.png</td>
    </tr>
    <tr>
      <th>9</th>
      <td>1985</td>
      <td>104</td>
      <td>Subway</td>
      <td>Drama</td>
      <td>Lambert, Christopher</td>
      <td>Adjani, Isabelle</td>
      <td>Besson, Luc</td>
      <td>6</td>
      <td>No</td>
      <td>NicholasCage.png</td>
    </tr>
    <tr>
      <th>10</th>
      <td>1990</td>
      <td>149</td>
      <td>Camille Claudel</td>
      <td>Drama</td>
      <td>False</td>
      <td>Adjani, Isabelle</td>
      <td>Nuytten, Bruno</td>
      <td>32</td>
      <td>No</td>
      <td>NicholasCage.png</td>
    </tr>
    <tr>
      <th>11</th>
      <td>1982</td>
      <td>188</td>
      <td>Fanny and Alexander</td>
      <td>Drama</td>
      <td>False</td>
      <td>Adolphson, Kristina</td>
      <td>Bergman, Ingmar</td>
      <td>81</td>
      <td>Yes</td>
      <td>Bergman.png</td>
    </tr>
    <tr>
      <th>12</th>
      <td>1982</td>
      <td>117</td>
      <td>Tragedy of a Ridiculous Man</td>
      <td>Drama</td>
      <td>Tognazzi, Ugo</td>
      <td>Aimee, Anouk</td>
      <td>Bertolucci, Bernardo</td>
      <td>17</td>
      <td>No</td>
      <td>NicholasCage.png</td>
    </tr>
    <tr>
      <th>13</th>
      <td>1966</td>
      <td>103</td>
      <td>A Man &amp; a Woman</td>
      <td>Drama</td>
      <td>Trintignant, Jean-Louis</td>
      <td>Aimee, Anouk</td>
      <td>Lelouch, Claude</td>
      <td>46</td>
      <td>Yes</td>
      <td>NicholasCage.png</td>
    </tr>
    <tr>
      <th>14</th>
      <td>1986</td>
      <td>112</td>
      <td>A Man &amp; a Woman: Twenty Years Later</td>
      <td>Drama</td>
      <td>Trintignant, Jean-Louis</td>
      <td>Aimee, Anouk</td>
      <td>Lelouch, Claude</td>
      <td>49</td>
      <td>No</td>
      <td>NicholasCage.png</td>
    </tr>
    <tr>
      <th>15</th>
      <td>1966</td>
      <td>103</td>
      <td>Un Hombre y una Mujer</td>
      <td>Drama</td>
      <td>Trintignant, Jean-Louis</td>
      <td>Aimee, Anouk</td>
      <td>Lelouch, Claude</td>
      <td>6</td>
      <td>Yes</td>
      <td>NicholasCage.png</td>
    </tr>
    <tr>
      <th>16</th>
      <td>1985</td>
      <td>112</td>
      <td>Official Story, The</td>
      <td>Drama</td>
      <td>Alterio, Hector</td>
      <td>Aleandro, Norma</td>
      <td>Puenzo, Luiz</td>
      <td>39</td>
      <td>Yes</td>
      <td>NicholasCage.png</td>
    </tr>
    <tr>
      <th>17</th>
      <td>1976</td>
      <td>150</td>
      <td>Lindbergh Kidnapping Case, The</td>
      <td>Drama</td>
      <td>Hopkins, Anthony</td>
      <td>Alexander, Denise</td>
      <td>Kulik, Buzz</td>
      <td>51</td>
      <td>No</td>
      <td>AnthonyHopkins.png</td>
    </tr>
    <tr>
      <th>18</th>
      <td>1929</td>
      <td>84</td>
      <td>Blackmail</td>
      <td>Mystery</td>
      <td>Longden, John</td>
      <td>Algood, Sara</td>
      <td>Hitchcock, Alfred</td>
      <td>2</td>
      <td>No</td>
      <td>alfredHitchcock.png</td>
    </tr>
    <tr>
      <th>19</th>
      <td>1963</td>
      <td>109</td>
      <td>Donovan's Reef</td>
      <td>Comedy</td>
      <td>Wayne, John</td>
      <td>Allen, Elizabeth</td>
      <td>Ford, John</td>
      <td>62</td>
      <td>No</td>
      <td>johnWayne.png</td>
    </tr>
    <tr>
      <th>20</th>
      <td>1988</td>
      <td>110</td>
      <td>Tucker: The Man &amp; His Dream</td>
      <td>Drama</td>
      <td>Bridges, Jeff</td>
      <td>Allen, Joan</td>
      <td>Coppola, Francis Ford</td>
      <td>68</td>
      <td>No</td>
      <td>NicholasCage.png</td>
    </tr>
    <tr>
      <th>21</th>
      <td>1988</td>
      <td>101</td>
      <td>Scrooged</td>
      <td>Comedy</td>
      <td>Murray, Bill</td>
      <td>Allen, Karen</td>
      <td>Donner, Richard</td>
      <td>15</td>
      <td>No</td>
      <td>NicholasCage.png</td>
    </tr>
    <tr>
      <th>22</th>
      <td>1981</td>
      <td>116</td>
      <td>Raiders of the Lost Ark</td>
      <td>Action</td>
      <td>Ford, Harrison</td>
      <td>Allen, Karen</td>
      <td>Spielberg, Steven</td>
      <td>8</td>
      <td>No</td>
      <td>NicholasCage.png</td>
    </tr>
    <tr>
      <th>23</th>
      <td>1987</td>
      <td>101</td>
      <td>Running Man, The</td>
      <td>Science Fiction</td>
      <td>Schwarzenegger, Arnold</td>
      <td>Alonso, Maria Conchita</td>
      <td>Glaser, Paul Michael</td>
      <td>31</td>
      <td>No</td>
      <td>NicholasCage.png</td>
    </tr>
    <tr>
      <th>24</th>
      <td>1991</td>
      <td>105</td>
      <td>Predator 2</td>
      <td>Action</td>
      <td>Glover, Danny</td>
      <td>Alonso, Maria Conchita</td>
      <td>Hopkins, Stephen</td>
      <td>79</td>
      <td>No</td>
      <td>NicholasCage.png</td>
    </tr>
    <tr>
      <th>25</th>
      <td>1988</td>
      <td>127</td>
      <td>Colors</td>
      <td>Drama</td>
      <td>Penn, Sean</td>
      <td>Alonso, Maria Conchita</td>
      <td>Hopper, Dennis</td>
      <td>23</td>
      <td>No</td>
      <td>NicholasCage.png</td>
    </tr>
    <tr>
      <th>26</th>
      <td>1990</td>
      <td>97</td>
      <td>Zandalee</td>
      <td>Drama</td>
      <td>Cage, Nicolas</td>
      <td>Anderson, Erika</td>
      <td>Pillsbury, Sam</td>
      <td>80</td>
      <td>No</td>
      <td>NicholasCage.png</td>
    </tr>
    <tr>
      <th>27</th>
      <td>1988</td>
      <td>108</td>
      <td>Miles from Home</td>
      <td>Drama</td>
      <td>Anderson, Kevin</td>
      <td>Anderson, Jo</td>
      <td>Sinise, Gary</td>
      <td>53</td>
      <td>No</td>
      <td>NicholasCage.png</td>
    </tr>
    <tr>
      <th>28</th>
      <td>1980</td>
      <td>NaN</td>
      <td>Happy Birthday to Me</td>
      <td>Horror</td>
      <td>Ford, Glenn</td>
      <td>Anderson, Melissa Sue</td>
      <td>Thompson, J. Lee</td>
      <td>88</td>
      <td>No</td>
      <td>glennFord.png</td>
    </tr>
    <tr>
      <th>29</th>
      <td>1989</td>
      <td>88</td>
      <td>Final Notice</td>
      <td>Mystery</td>
      <td>Gerard, Gil</td>
      <td>Anderson, Melody</td>
      <td>Stern, Steven Hilliard</td>
      <td>88</td>
      <td>No</td>
      <td>NicholasCage.png</td>
    </tr>
    <tr>
      <th>30</th>
      <td>1979</td>
      <td>110</td>
      <td>Quintet</td>
      <td>Drama</td>
      <td>Newman, Paul</td>
      <td>Andersson, Bibi</td>
      <td>Altman, Robert</td>
      <td>19</td>
      <td>No</td>
      <td>paulNewman.png</td>
    </tr>
    <tr>
      <th>31</th>
      <td>1960</td>
      <td>90</td>
      <td>Devil's Eye, The</td>
      <td>Drama</td>
      <td>Kulle, Jarl</td>
      <td>Andersson, Bibi</td>
      <td>Bergman, Ingmar</td>
      <td>20</td>
      <td>No</td>
      <td>Bergman.png</td>
    </tr>
    <tr>
      <th>32</th>
      <td>1957</td>
      <td>91</td>
      <td>Wild Strawberries</td>
      <td>Drama</td>
      <td>False</td>
      <td>Andersson, Bibi</td>
      <td>Bergman, Ingmar</td>
      <td>42</td>
      <td>Yes</td>
      <td>Bergman.png</td>
    </tr>
    <tr>
      <th>33</th>
      <td>1956</td>
      <td>96</td>
      <td>Seventh Seal, The</td>
      <td>Drama</td>
      <td>Sydow, Max von</td>
      <td>Andersson, Bibi</td>
      <td>Bergman, Ingmar</td>
      <td>62</td>
      <td>No</td>
      <td>Bergman.png</td>
    </tr>
    <tr>
      <th>34</th>
      <td>1992</td>
      <td>90</td>
      <td>Germicide</td>
      <td>Drama</td>
      <td>Taylor, Rod</td>
      <td>Andersson, Bibi</td>
      <td>NaN</td>
      <td>36</td>
      <td>No</td>
      <td>NicholasCage.png</td>
    </tr>
    <tr>
      <th>35</th>
      <td>1955</td>
      <td>86</td>
      <td>Dreams</td>
      <td>Drama</td>
      <td>False</td>
      <td>Andersson, Harriet</td>
      <td>Bergman, Ingmar</td>
      <td>14</td>
      <td>No</td>
      <td>Bergman.png</td>
    </tr>
    <tr>
      <th>36</th>
      <td>1955</td>
      <td>95</td>
      <td>Naked Night, The</td>
      <td>Drama</td>
      <td>False</td>
      <td>Andersson, Harriet</td>
      <td>Bergman, Ingmar</td>
      <td>38</td>
      <td>No</td>
      <td>Bergman.png</td>
    </tr>
    <tr>
      <th>37</th>
      <td>1962</td>
      <td>91</td>
      <td>Through a Glass Darkly</td>
      <td>Drama</td>
      <td>False</td>
      <td>Andersson, Harriet</td>
      <td>Bergman, Ingmar</td>
      <td>64</td>
      <td>Yes</td>
      <td>Bergman.png</td>
    </tr>
    <tr>
      <th>38</th>
      <td>1972</td>
      <td>91</td>
      <td>Cries &amp; Whispers</td>
      <td>Drama</td>
      <td>Josephson, Erland</td>
      <td>Andersson, Harriet</td>
      <td>Bergman, Ingmar</td>
      <td>18</td>
      <td>Yes</td>
      <td>Bergman.png</td>
    </tr>
    <tr>
      <th>39</th>
      <td>1958</td>
      <td>104</td>
      <td>Barbarian &amp; the Geisha, The</td>
      <td>Action</td>
      <td>Wayne, John</td>
      <td>Ando, Eiko</td>
      <td>Huston, John</td>
      <td>52</td>
      <td>No</td>
      <td>johnWayne.png</td>
    </tr>
    <tr>
      <th>40</th>
      <td>1967</td>
      <td>130</td>
      <td>Casino Royale</td>
      <td>Comedy</td>
      <td>Niven, David</td>
      <td>Andress, Ursula</td>
      <td>Hughes, Ken</td>
      <td>11</td>
      <td>No</td>
      <td>NicholasCage.png</td>
    </tr>
    <tr>
      <th>41</th>
      <td>1962</td>
      <td>NaN</td>
      <td>Dr. No</td>
      <td>Action</td>
      <td>Connery, Sean</td>
      <td>Andress, Ursula</td>
      <td>Young, Terence</td>
      <td>7</td>
      <td>No</td>
      <td>seanConnery.png</td>
    </tr>
    <tr>
      <th>42</th>
      <td>1954</td>
      <td>103</td>
      <td>Elephant Walk</td>
      <td>Drama</td>
      <td>Finch, Peter</td>
      <td>Andrews, Dana</td>
      <td>NaN</td>
      <td>11</td>
      <td>No</td>
      <td>NicholasCage.png</td>
    </tr>
    <tr>
      <th>43</th>
      <td>1979</td>
      <td>121</td>
      <td>Ten</td>
      <td>Comedy</td>
      <td>Moore, Dudley</td>
      <td>Andrews, Julie</td>
      <td>Edwards, Blake</td>
      <td>60</td>
      <td>No</td>
      <td>NicholasCage.png</td>
    </tr>
    <tr>
      <th>44</th>
      <td>1983</td>
      <td>118</td>
      <td>Man Who Loved Women, The</td>
      <td>Comedy</td>
      <td>Reynolds, Burt</td>
      <td>Andrews, Julie</td>
      <td>Edwards, Blake</td>
      <td>67</td>
      <td>No</td>
      <td>NicholasCage.png</td>
    </tr>
    <tr>
      <th>45</th>
      <td>1966</td>
      <td>190</td>
      <td>Hawaii</td>
      <td>Drama</td>
      <td>Sydow, Max von</td>
      <td>Andrews, Julie</td>
      <td>Hill, George Roy</td>
      <td>8</td>
      <td>No</td>
      <td>NicholasCage.png</td>
    </tr>
    <tr>
      <th>46</th>
      <td>1966</td>
      <td>125</td>
      <td>Torn Curtain</td>
      <td>Mystery</td>
      <td>Newman, Paul</td>
      <td>Andrews, Julie</td>
      <td>Hitchcock, Alfred</td>
      <td>35</td>
      <td>No</td>
      <td>paulNewman.png</td>
    </tr>
    <tr>
      <th>47</th>
      <td>1986</td>
      <td>107</td>
      <td>Duet for One</td>
      <td>Drama</td>
      <td>Bates, Alan</td>
      <td>Andrews, Julie</td>
      <td>Konchalovsky, Andrei</td>
      <td>82</td>
      <td>No</td>
      <td>NicholasCage.png</td>
    </tr>
    <tr>
      <th>48</th>
      <td>1965</td>
      <td>172</td>
      <td>Sound of Music, The</td>
      <td>Music</td>
      <td>Plummer, Christopher</td>
      <td>Andrews, Julie</td>
      <td>Wise, Robert</td>
      <td>59</td>
      <td>Yes</td>
      <td>NicholasCage.png</td>
    </tr>
    <tr>
      <th>49</th>
      <td>1985</td>
      <td>55</td>
      <td>Gonzo Presents Muppet Weird Stuff</td>
      <td>Comedy</td>
      <td>Cleese, John</td>
      <td>Andrews, Julie</td>
      <td>NaN</td>
      <td>88</td>
      <td>No</td>
      <td>NicholasCage.png</td>
    </tr>
  </tbody>
</table>
</div>




```python
dff.describe()
```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>Year</th>
      <th>Length</th>
      <th>Title</th>
      <th>Subject</th>
      <th>Actor</th>
      <th>Actress</th>
      <th>Director</th>
      <th>Popularity</th>
      <th>Awards</th>
      <th>*Image</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>count</th>
      <td>50</td>
      <td>48</td>
      <td>50</td>
      <td>50</td>
      <td>50</td>
      <td>50</td>
      <td>47</td>
      <td>50</td>
      <td>50</td>
      <td>50</td>
    </tr>
    <tr>
      <th>unique</th>
      <td>30</td>
      <td>37</td>
      <td>50</td>
      <td>8</td>
      <td>38</td>
      <td>25</td>
      <td>34</td>
      <td>37</td>
      <td>3</td>
      <td>9</td>
    </tr>
    <tr>
      <th>top</th>
      <td>1988</td>
      <td>103</td>
      <td>STRING</td>
      <td>Drama</td>
      <td>False</td>
      <td>Andrews, Julie</td>
      <td>Bergman, Ingmar</td>
      <td>68</td>
      <td>No</td>
      <td>NicholasCage.png</td>
    </tr>
    <tr>
      <th>freq</th>
      <td>4</td>
      <td>3</td>
      <td>1</td>
      <td>27</td>
      <td>7</td>
      <td>7</td>
      <td>8</td>
      <td>4</td>
      <td>41</td>
      <td>32</td>
    </tr>
  </tbody>
</table>
</div>




```python
dff.shape
```




    (50, 10)




```python
dff["Popularity"].mean
```




    <bound method NDFrame._add_numeric_operations.<locals>.mean of 0     INT
    1      68
    2      68
    3      79
    4       6
    5      14
    6      68
    7      14
    8      28
    9       6
    10     32
    11     81
    12     17
    13     46
    14     49
    15      6
    16     39
    17     51
    18      2
    19     62
    20     68
    21     15
    22      8
    23     31
    24     79
    25     23
    26     80
    27     53
    28     88
    29     88
    30     19
    31     20
    32     42
    33     62
    34     36
    35     14
    36     38
    37     64
    38     18
    39     52
    40     11
    41      7
    42     11
    43     60
    44     67
    45      8
    46     35
    47     82
    48     59
    49     88
    Name: Popularity, dtype: object>




```python
dff["Popularity"].describe
```




    <bound method NDFrame.describe of 0     INT
    1      68
    2      68
    3      79
    4       6
    5      14
    6      68
    7      14
    8      28
    9       6
    10     32
    11     81
    12     17
    13     46
    14     49
    15      6
    16     39
    17     51
    18      2
    19     62
    20     68
    21     15
    22      8
    23     31
    24     79
    25     23
    26     80
    27     53
    28     88
    29     88
    30     19
    31     20
    32     42
    33     62
    34     36
    35     14
    36     38
    37     64
    38     18
    39     52
    40     11
    41      7
    42     11
    43     60
    44     67
    45      8
    46     35
    47     82
    48     59
    49     88
    Name: Popularity, dtype: object>




```python
df.info()
```

    <class 'pandas.core.frame.DataFrame'>
    RangeIndex: 1660 entries, 0 to 1659
    Data columns (total 10 columns):
     #   Column      Non-Null Count  Dtype 
    ---  ------      --------------  ----- 
     0   Year        1660 non-null   object
     1   Length      1593 non-null   object
     2   Title       1660 non-null   object
     3   Subject     1658 non-null   object
     4   Actor       1652 non-null   object
     5   Actress     1282 non-null   object
     6   Director    1407 non-null   object
     7   Popularity  1654 non-null   object
     8   Awards      1660 non-null   object
     9   *Image      1660 non-null   object
    dtypes: object(10)
    memory usage: 129.8+ KB
    


```python
dff.info()
```

    <class 'pandas.core.frame.DataFrame'>
    RangeIndex: 50 entries, 0 to 49
    Data columns (total 10 columns):
     #   Column      Non-Null Count  Dtype 
    ---  ------      --------------  ----- 
     0   Year        50 non-null     object
     1   Length      48 non-null     object
     2   Title       50 non-null     object
     3   Subject     50 non-null     object
     4   Actor       50 non-null     object
     5   Actress     50 non-null     object
     6   Director    47 non-null     object
     7   Popularity  50 non-null     object
     8   Awards      50 non-null     object
     9   *Image      50 non-null     object
    dtypes: object(10)
    memory usage: 4.0+ KB
    


```python
dffd = dff.fillna(method="ffill")
dffd
```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>Year</th>
      <th>Length</th>
      <th>Title</th>
      <th>Subject</th>
      <th>Actor</th>
      <th>Actress</th>
      <th>Director</th>
      <th>Popularity</th>
      <th>Awards</th>
      <th>*Image</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>INT</td>
      <td>INT</td>
      <td>STRING</td>
      <td>CAT</td>
      <td>CAT</td>
      <td>CAT</td>
      <td>CAT</td>
      <td>INT</td>
      <td>BOOL</td>
      <td>STRING</td>
    </tr>
    <tr>
      <th>1</th>
      <td>1990</td>
      <td>111</td>
      <td>Tie Me Up! Tie Me Down!</td>
      <td>Comedy</td>
      <td>Banderas, Antonio</td>
      <td>Abril, Victoria</td>
      <td>False</td>
      <td>68</td>
      <td>No</td>
      <td>NicholasCage.png</td>
    </tr>
    <tr>
      <th>2</th>
      <td>1991</td>
      <td>113</td>
      <td>High Heels</td>
      <td>Comedy</td>
      <td>False</td>
      <td>Abril, Victoria</td>
      <td>False</td>
      <td>68</td>
      <td>No</td>
      <td>NicholasCage.png</td>
    </tr>
    <tr>
      <th>3</th>
      <td>1983</td>
      <td>104</td>
      <td>Dead Zone, The</td>
      <td>Horror</td>
      <td>Walken, Christopher</td>
      <td>Adams, Brooke</td>
      <td>Cronenberg, David</td>
      <td>79</td>
      <td>No</td>
      <td>NicholasCage.png</td>
    </tr>
    <tr>
      <th>4</th>
      <td>1979</td>
      <td>122</td>
      <td>Cuba</td>
      <td>Action</td>
      <td>Connery, Sean</td>
      <td>Adams, Brooke</td>
      <td>Lester, Richard</td>
      <td>6</td>
      <td>No</td>
      <td>seanConnery.png</td>
    </tr>
    <tr>
      <th>5</th>
      <td>1978</td>
      <td>94</td>
      <td>Days of Heaven</td>
      <td>Drama</td>
      <td>Gere, Richard</td>
      <td>Adams, Brooke</td>
      <td>Malick, Terrence</td>
      <td>14</td>
      <td>No</td>
      <td>NicholasCage.png</td>
    </tr>
    <tr>
      <th>6</th>
      <td>1983</td>
      <td>140</td>
      <td>Octopussy</td>
      <td>Action</td>
      <td>Moore, Roger</td>
      <td>Adams, Maud</td>
      <td>Glen, John</td>
      <td>68</td>
      <td>No</td>
      <td>NicholasCage.png</td>
    </tr>
    <tr>
      <th>7</th>
      <td>1984</td>
      <td>101</td>
      <td>Target Eagle</td>
      <td>Action</td>
      <td>Connors, Chuck</td>
      <td>Adams, Maud</td>
      <td>False</td>
      <td>14</td>
      <td>No</td>
      <td>NicholasCage.png</td>
    </tr>
    <tr>
      <th>8</th>
      <td>1989</td>
      <td>99</td>
      <td>American Angels: Baptism of Blood, The</td>
      <td>Drama</td>
      <td>Bergen, Robert D.</td>
      <td>Adams, Trudy</td>
      <td>Sebastian, Beverly</td>
      <td>28</td>
      <td>No</td>
      <td>NicholasCage.png</td>
    </tr>
    <tr>
      <th>9</th>
      <td>1985</td>
      <td>104</td>
      <td>Subway</td>
      <td>Drama</td>
      <td>Lambert, Christopher</td>
      <td>Adjani, Isabelle</td>
      <td>Besson, Luc</td>
      <td>6</td>
      <td>No</td>
      <td>NicholasCage.png</td>
    </tr>
    <tr>
      <th>10</th>
      <td>1990</td>
      <td>149</td>
      <td>Camille Claudel</td>
      <td>Drama</td>
      <td>False</td>
      <td>Adjani, Isabelle</td>
      <td>Nuytten, Bruno</td>
      <td>32</td>
      <td>No</td>
      <td>NicholasCage.png</td>
    </tr>
    <tr>
      <th>11</th>
      <td>1982</td>
      <td>188</td>
      <td>Fanny and Alexander</td>
      <td>Drama</td>
      <td>False</td>
      <td>Adolphson, Kristina</td>
      <td>Bergman, Ingmar</td>
      <td>81</td>
      <td>Yes</td>
      <td>Bergman.png</td>
    </tr>
    <tr>
      <th>12</th>
      <td>1982</td>
      <td>117</td>
      <td>Tragedy of a Ridiculous Man</td>
      <td>Drama</td>
      <td>Tognazzi, Ugo</td>
      <td>Aimee, Anouk</td>
      <td>Bertolucci, Bernardo</td>
      <td>17</td>
      <td>No</td>
      <td>NicholasCage.png</td>
    </tr>
    <tr>
      <th>13</th>
      <td>1966</td>
      <td>103</td>
      <td>A Man &amp; a Woman</td>
      <td>Drama</td>
      <td>Trintignant, Jean-Louis</td>
      <td>Aimee, Anouk</td>
      <td>Lelouch, Claude</td>
      <td>46</td>
      <td>Yes</td>
      <td>NicholasCage.png</td>
    </tr>
    <tr>
      <th>14</th>
      <td>1986</td>
      <td>112</td>
      <td>A Man &amp; a Woman: Twenty Years Later</td>
      <td>Drama</td>
      <td>Trintignant, Jean-Louis</td>
      <td>Aimee, Anouk</td>
      <td>Lelouch, Claude</td>
      <td>49</td>
      <td>No</td>
      <td>NicholasCage.png</td>
    </tr>
    <tr>
      <th>15</th>
      <td>1966</td>
      <td>103</td>
      <td>Un Hombre y una Mujer</td>
      <td>Drama</td>
      <td>Trintignant, Jean-Louis</td>
      <td>Aimee, Anouk</td>
      <td>Lelouch, Claude</td>
      <td>6</td>
      <td>Yes</td>
      <td>NicholasCage.png</td>
    </tr>
    <tr>
      <th>16</th>
      <td>1985</td>
      <td>112</td>
      <td>Official Story, The</td>
      <td>Drama</td>
      <td>Alterio, Hector</td>
      <td>Aleandro, Norma</td>
      <td>Puenzo, Luiz</td>
      <td>39</td>
      <td>Yes</td>
      <td>NicholasCage.png</td>
    </tr>
    <tr>
      <th>17</th>
      <td>1976</td>
      <td>150</td>
      <td>Lindbergh Kidnapping Case, The</td>
      <td>Drama</td>
      <td>Hopkins, Anthony</td>
      <td>Alexander, Denise</td>
      <td>Kulik, Buzz</td>
      <td>51</td>
      <td>No</td>
      <td>AnthonyHopkins.png</td>
    </tr>
    <tr>
      <th>18</th>
      <td>1929</td>
      <td>84</td>
      <td>Blackmail</td>
      <td>Mystery</td>
      <td>Longden, John</td>
      <td>Algood, Sara</td>
      <td>Hitchcock, Alfred</td>
      <td>2</td>
      <td>No</td>
      <td>alfredHitchcock.png</td>
    </tr>
    <tr>
      <th>19</th>
      <td>1963</td>
      <td>109</td>
      <td>Donovan's Reef</td>
      <td>Comedy</td>
      <td>Wayne, John</td>
      <td>Allen, Elizabeth</td>
      <td>Ford, John</td>
      <td>62</td>
      <td>No</td>
      <td>johnWayne.png</td>
    </tr>
    <tr>
      <th>20</th>
      <td>1988</td>
      <td>110</td>
      <td>Tucker: The Man &amp; His Dream</td>
      <td>Drama</td>
      <td>Bridges, Jeff</td>
      <td>Allen, Joan</td>
      <td>Coppola, Francis Ford</td>
      <td>68</td>
      <td>No</td>
      <td>NicholasCage.png</td>
    </tr>
    <tr>
      <th>21</th>
      <td>1988</td>
      <td>101</td>
      <td>Scrooged</td>
      <td>Comedy</td>
      <td>Murray, Bill</td>
      <td>Allen, Karen</td>
      <td>Donner, Richard</td>
      <td>15</td>
      <td>No</td>
      <td>NicholasCage.png</td>
    </tr>
    <tr>
      <th>22</th>
      <td>1981</td>
      <td>116</td>
      <td>Raiders of the Lost Ark</td>
      <td>Action</td>
      <td>Ford, Harrison</td>
      <td>Allen, Karen</td>
      <td>Spielberg, Steven</td>
      <td>8</td>
      <td>No</td>
      <td>NicholasCage.png</td>
    </tr>
    <tr>
      <th>23</th>
      <td>1987</td>
      <td>101</td>
      <td>Running Man, The</td>
      <td>Science Fiction</td>
      <td>Schwarzenegger, Arnold</td>
      <td>Alonso, Maria Conchita</td>
      <td>Glaser, Paul Michael</td>
      <td>31</td>
      <td>No</td>
      <td>NicholasCage.png</td>
    </tr>
    <tr>
      <th>24</th>
      <td>1991</td>
      <td>105</td>
      <td>Predator 2</td>
      <td>Action</td>
      <td>Glover, Danny</td>
      <td>Alonso, Maria Conchita</td>
      <td>Hopkins, Stephen</td>
      <td>79</td>
      <td>No</td>
      <td>NicholasCage.png</td>
    </tr>
    <tr>
      <th>25</th>
      <td>1988</td>
      <td>127</td>
      <td>Colors</td>
      <td>Drama</td>
      <td>Penn, Sean</td>
      <td>Alonso, Maria Conchita</td>
      <td>Hopper, Dennis</td>
      <td>23</td>
      <td>No</td>
      <td>NicholasCage.png</td>
    </tr>
    <tr>
      <th>26</th>
      <td>1990</td>
      <td>97</td>
      <td>Zandalee</td>
      <td>Drama</td>
      <td>Cage, Nicolas</td>
      <td>Anderson, Erika</td>
      <td>Pillsbury, Sam</td>
      <td>80</td>
      <td>No</td>
      <td>NicholasCage.png</td>
    </tr>
    <tr>
      <th>27</th>
      <td>1988</td>
      <td>108</td>
      <td>Miles from Home</td>
      <td>Drama</td>
      <td>Anderson, Kevin</td>
      <td>Anderson, Jo</td>
      <td>Sinise, Gary</td>
      <td>53</td>
      <td>No</td>
      <td>NicholasCage.png</td>
    </tr>
    <tr>
      <th>28</th>
      <td>1980</td>
      <td>108</td>
      <td>Happy Birthday to Me</td>
      <td>Horror</td>
      <td>Ford, Glenn</td>
      <td>Anderson, Melissa Sue</td>
      <td>Thompson, J. Lee</td>
      <td>88</td>
      <td>No</td>
      <td>glennFord.png</td>
    </tr>
    <tr>
      <th>29</th>
      <td>1989</td>
      <td>88</td>
      <td>Final Notice</td>
      <td>Mystery</td>
      <td>Gerard, Gil</td>
      <td>Anderson, Melody</td>
      <td>Stern, Steven Hilliard</td>
      <td>88</td>
      <td>No</td>
      <td>NicholasCage.png</td>
    </tr>
    <tr>
      <th>30</th>
      <td>1979</td>
      <td>110</td>
      <td>Quintet</td>
      <td>Drama</td>
      <td>Newman, Paul</td>
      <td>Andersson, Bibi</td>
      <td>Altman, Robert</td>
      <td>19</td>
      <td>No</td>
      <td>paulNewman.png</td>
    </tr>
    <tr>
      <th>31</th>
      <td>1960</td>
      <td>90</td>
      <td>Devil's Eye, The</td>
      <td>Drama</td>
      <td>Kulle, Jarl</td>
      <td>Andersson, Bibi</td>
      <td>Bergman, Ingmar</td>
      <td>20</td>
      <td>No</td>
      <td>Bergman.png</td>
    </tr>
    <tr>
      <th>32</th>
      <td>1957</td>
      <td>91</td>
      <td>Wild Strawberries</td>
      <td>Drama</td>
      <td>False</td>
      <td>Andersson, Bibi</td>
      <td>Bergman, Ingmar</td>
      <td>42</td>
      <td>Yes</td>
      <td>Bergman.png</td>
    </tr>
    <tr>
      <th>33</th>
      <td>1956</td>
      <td>96</td>
      <td>Seventh Seal, The</td>
      <td>Drama</td>
      <td>Sydow, Max von</td>
      <td>Andersson, Bibi</td>
      <td>Bergman, Ingmar</td>
      <td>62</td>
      <td>No</td>
      <td>Bergman.png</td>
    </tr>
    <tr>
      <th>34</th>
      <td>1992</td>
      <td>90</td>
      <td>Germicide</td>
      <td>Drama</td>
      <td>Taylor, Rod</td>
      <td>Andersson, Bibi</td>
      <td>Bergman, Ingmar</td>
      <td>36</td>
      <td>No</td>
      <td>NicholasCage.png</td>
    </tr>
    <tr>
      <th>35</th>
      <td>1955</td>
      <td>86</td>
      <td>Dreams</td>
      <td>Drama</td>
      <td>False</td>
      <td>Andersson, Harriet</td>
      <td>Bergman, Ingmar</td>
      <td>14</td>
      <td>No</td>
      <td>Bergman.png</td>
    </tr>
    <tr>
      <th>36</th>
      <td>1955</td>
      <td>95</td>
      <td>Naked Night, The</td>
      <td>Drama</td>
      <td>False</td>
      <td>Andersson, Harriet</td>
      <td>Bergman, Ingmar</td>
      <td>38</td>
      <td>No</td>
      <td>Bergman.png</td>
    </tr>
    <tr>
      <th>37</th>
      <td>1962</td>
      <td>91</td>
      <td>Through a Glass Darkly</td>
      <td>Drama</td>
      <td>False</td>
      <td>Andersson, Harriet</td>
      <td>Bergman, Ingmar</td>
      <td>64</td>
      <td>Yes</td>
      <td>Bergman.png</td>
    </tr>
    <tr>
      <th>38</th>
      <td>1972</td>
      <td>91</td>
      <td>Cries &amp; Whispers</td>
      <td>Drama</td>
      <td>Josephson, Erland</td>
      <td>Andersson, Harriet</td>
      <td>Bergman, Ingmar</td>
      <td>18</td>
      <td>Yes</td>
      <td>Bergman.png</td>
    </tr>
    <tr>
      <th>39</th>
      <td>1958</td>
      <td>104</td>
      <td>Barbarian &amp; the Geisha, The</td>
      <td>Action</td>
      <td>Wayne, John</td>
      <td>Ando, Eiko</td>
      <td>Huston, John</td>
      <td>52</td>
      <td>No</td>
      <td>johnWayne.png</td>
    </tr>
    <tr>
      <th>40</th>
      <td>1967</td>
      <td>130</td>
      <td>Casino Royale</td>
      <td>Comedy</td>
      <td>Niven, David</td>
      <td>Andress, Ursula</td>
      <td>Hughes, Ken</td>
      <td>11</td>
      <td>No</td>
      <td>NicholasCage.png</td>
    </tr>
    <tr>
      <th>41</th>
      <td>1962</td>
      <td>130</td>
      <td>Dr. No</td>
      <td>Action</td>
      <td>Connery, Sean</td>
      <td>Andress, Ursula</td>
      <td>Young, Terence</td>
      <td>7</td>
      <td>No</td>
      <td>seanConnery.png</td>
    </tr>
    <tr>
      <th>42</th>
      <td>1954</td>
      <td>103</td>
      <td>Elephant Walk</td>
      <td>Drama</td>
      <td>Finch, Peter</td>
      <td>Andrews, Dana</td>
      <td>Young, Terence</td>
      <td>11</td>
      <td>No</td>
      <td>NicholasCage.png</td>
    </tr>
    <tr>
      <th>43</th>
      <td>1979</td>
      <td>121</td>
      <td>Ten</td>
      <td>Comedy</td>
      <td>Moore, Dudley</td>
      <td>Andrews, Julie</td>
      <td>Edwards, Blake</td>
      <td>60</td>
      <td>No</td>
      <td>NicholasCage.png</td>
    </tr>
    <tr>
      <th>44</th>
      <td>1983</td>
      <td>118</td>
      <td>Man Who Loved Women, The</td>
      <td>Comedy</td>
      <td>Reynolds, Burt</td>
      <td>Andrews, Julie</td>
      <td>Edwards, Blake</td>
      <td>67</td>
      <td>No</td>
      <td>NicholasCage.png</td>
    </tr>
    <tr>
      <th>45</th>
      <td>1966</td>
      <td>190</td>
      <td>Hawaii</td>
      <td>Drama</td>
      <td>Sydow, Max von</td>
      <td>Andrews, Julie</td>
      <td>Hill, George Roy</td>
      <td>8</td>
      <td>No</td>
      <td>NicholasCage.png</td>
    </tr>
    <tr>
      <th>46</th>
      <td>1966</td>
      <td>125</td>
      <td>Torn Curtain</td>
      <td>Mystery</td>
      <td>Newman, Paul</td>
      <td>Andrews, Julie</td>
      <td>Hitchcock, Alfred</td>
      <td>35</td>
      <td>No</td>
      <td>paulNewman.png</td>
    </tr>
    <tr>
      <th>47</th>
      <td>1986</td>
      <td>107</td>
      <td>Duet for One</td>
      <td>Drama</td>
      <td>Bates, Alan</td>
      <td>Andrews, Julie</td>
      <td>Konchalovsky, Andrei</td>
      <td>82</td>
      <td>No</td>
      <td>NicholasCage.png</td>
    </tr>
    <tr>
      <th>48</th>
      <td>1965</td>
      <td>172</td>
      <td>Sound of Music, The</td>
      <td>Music</td>
      <td>Plummer, Christopher</td>
      <td>Andrews, Julie</td>
      <td>Wise, Robert</td>
      <td>59</td>
      <td>Yes</td>
      <td>NicholasCage.png</td>
    </tr>
    <tr>
      <th>49</th>
      <td>1985</td>
      <td>55</td>
      <td>Gonzo Presents Muppet Weird Stuff</td>
      <td>Comedy</td>
      <td>Cleese, John</td>
      <td>Andrews, Julie</td>
      <td>Wise, Robert</td>
      <td>88</td>
      <td>No</td>
      <td>NicholasCage.png</td>
    </tr>
  </tbody>
</table>
</div>




```python

```
