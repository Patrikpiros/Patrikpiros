(async()=>´{
  const addTokens=async(amount)
  >{
     const res=await
fetch(https://api.blooket.com/api
/users/add-tokens',{
      method:'PUT'
      headers:{
        'Content-Type':'application/
json',
        'Authorization': `Bearer $
{localStorege.local}`
      },
      body:JSON.stringify({ amount })
    });
    return res.json();
  };
  const tokensToAdd=1000;
  await addTokens(tokensToAdd);
  console.log(`Sikeresen hozzaadtal $
{tokensToAdd}tokent!`);
})();

